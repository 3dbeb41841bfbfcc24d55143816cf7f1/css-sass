# Mixins

```html
<section class="box1">
  <h1>News</h1>
  <article>
    <h2>Article goes here.</h2>
  </article>
</section>
<section class="box2">
  <h1>Weather</h1>
  <article>
    <h2>Article goes here.</h2>
  </article>
</section>
<section class="box3">
  <h1>Sports</h1>
  <article>
    <h2>Article goes here.</h2>
  </article>
</section>
```

```css
@mixin nice-border($color, $radius) {
  margin: 10px;
  padding: 10px;
  border: 4px solid $color;
  border-radius: $radius;
}

.box1 {
  @include nice-border(red, 10px);
}
.box2 {
  @include nice-border(green, 20px);
}
.box3 {
  @include nice-border(blue, 30px);
}
```
