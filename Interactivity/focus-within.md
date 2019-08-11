# Focus Within

> https://30-seconds.github.io/30-seconds-of-css/#focus-within

Changes the appearance of a form if any of its children are focused.

HTML

```html
<div class="focus-within">
  <form>
    <label for="given_name">Given Name:</label> <input id="given_name" type="text" /> <br />
    <label for="family_name">Family Name:</label> <input id="family_name" type="text" />
  </form>
</div>
```

CSS

```css
form {
  border: 3px solid #2d98da;
  color: #000000;
  padding: 4px;
}
form:focus-within {
  background: #f7b731;
  color: #000000;
}
```

#### Explanation

The psuedo class `:focus-within` applies styles to a parent element if any child element gets focused. For example, an `input` element inside a `form` element.

