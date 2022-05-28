## Color Picker

<iframe width="560" height="315" src="https://www.youtube.com/embed/6bS4E8bD8hU" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Create a color picker with 2 components.  One component should contain the slider and the label.  The other component will be a div to display the color.  Use prop binding and reactive variables to make your application dynamic.

## Code Copy

```js
const rgbToHex = function (rgb) {
  var hex = Number(rgb).toString(16);
  if (hex.length < 2) {
    hex = "0" + hex;
  }
  return hex;
};
 
export const fullColorHex = function (r, g, b) {
  var red = rgbToHex(r);
  var green = rgbToHex(g);
  var blue = rgbToHex(b);
  return "#" + red + green + blue;
};
```

## Learning Goals

- Reactive Variables
- Props and prop binding

## Resource

- [Discord](https://discord.gg/Jwv7xaPRMS)
- [Prop Binding](https://svelte.dev/examples/component-bindings)
- [Reactive Variables](https://svelte.dev/examples/reactive-declarations)


