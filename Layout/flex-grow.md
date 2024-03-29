# Last item with remaining available height

> https://30-seconds.github.io/30-seconds-of-css/#last-item-with-remaining-available-height

Take advantage of available viewport space by giving the last element the remaining available space in current viewport, even when resizing the window.

HTML

```html
<div class="container">
  <div>Div 1</div>
  <div>Div 2</div>
  <div>Div 3</div>
</div>
```

CSS

```css
html,
body {
  height: 100%;
  margin: 0;
}
.container {
  height: 100%;
  display: flex;
  flex-direction: column;
}
.container > div:last-child {
  background-color: tomato;
  flex: 1;
}
```

#### Explanation

1. `height: 100%` set the height of container as viewport height.
2. `display: flex` enables flexbox.
3. `flex-direction: column` set the direction of flex items' order from top to down.
4. `flex-grow: 1` the flexbox will apply remaining available space of container to last child element.

The parent must have a viewport height. `flex-grow: 1` could be applied to the first or second element, which will have all available space.

最后一个 `div`  可以占满窗口整个剩余区域。

