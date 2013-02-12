# Julep

SASS/SCSS mixins for building mobile web applications. Designed to keep your markup clean and semantic and free of cruft.

## Requirements

* Bourbon (http://bourbon.io)

## Installation

* Clone the repository to your stylesheets directory.

* Add `@import "julep/julep"` to your SASS/SCSS.

## Usage

Simply include the appropriate mixin in your stylesheet. E.g.

### Header

```html
<header>
  <h1>App Name</h1>
</header>
```

```css
header {
  @include header($color);
}
```

### Tab Bar

Pass the number of buttons in your tab bar to the mixin.

```html
<footer>
  <ul>
    <li><a href="#" id="one">One</a></li>
    <li><a href="#" id="two">Two</a></li>
  </ul>
</footer>
```

```css
footer {
  @include tabbar(2);
}
```

### Lists

```html
<ul>
  <li>First Item</li>
  <li>Second Item</li>
  <li>Third Item</li>
</ul>
```

```css
ul {
  @include list;
}
```

## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Added some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request
