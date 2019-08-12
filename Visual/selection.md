# Custom text selection

> https://30-seconds.github.io/30-seconds-of-css/#custom-text-selection

Changes the styling of text selection.

改变选中文本的原有样式。

HTML

```html
<p class="custom-text-selection">Select some of this text.</p>
```

CSS

```css
::selection {
  background: aquamarine;
  color: black;
}
.custom-text-selection::selection {
  background: deeppink;
  color: white;
}
```

#### Explanation

`::selection` defines a pseudo selector on an element to style text within it when selected. Note that if you don't combine any other selector your style will be applied at document root level, to any selectable element.



