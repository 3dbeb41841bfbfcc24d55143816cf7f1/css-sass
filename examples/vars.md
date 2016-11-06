# Variables and Color Functions

```html
<h1>This is a level 1 heading</h1>
<h2>This is a level 2 heading</h2>
<p>This is a paragraph</p>
<button>I am a button, click Me!</button>
```

```css
$base-color: #AD141E;
$button-fg-color: yellow;
$button-bg-color: blue;
$color-amount: 10%;

p {
  color: $base-color;
}
h1 {
  color: darken( $base-color, $color-amount );
}
h2 {
  color: lighten( $base-color, $color-amount );
}
button {
  color: $button-fg-color;
  background-color: $button-bg-color;
  &:hover {
    color: invert($button-fg-color);
    background-color: invert($button-bg-color);
  }
}
```
