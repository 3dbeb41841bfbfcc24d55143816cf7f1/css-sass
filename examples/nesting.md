# Nesting

```html
<nav>
  <ul>
    <li><a href="#news">News</a></li>
    <li><a href="#weather">Weather</a></li>
    <li><a href="#sports">Sports</a></li>
  </ul>
</nav>

<h2>Here is some fruit</h2>
<ul>
  <li>Apple</li>
  <li>Orange</li>
  <li>Banana</li>
</ul>
```

```css
nav {
  ul {
    margin: 0;
    padding: 0;
    list-style: none;
  }

  li { display: inline-block; }

  a {
    display: block;
    padding: 6px 12px;
    text-decoration: none;
  }
}
```
