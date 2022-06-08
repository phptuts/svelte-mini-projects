# Color Picker

<iframe width="560" height="315" src="https://www.youtube.com/embed/ZbhkMSDKEyA" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Create a color picker with 2 components.  One component should contain the slider and the label.  The other component will be a div to display the color.  Use the useEffect how to make it so that the hex color value is create updates the div component.  

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

- How to create components and pass in props
- How to make your components reactive with useEffect
- Practice useState
- Practice Events

## [Code](https://codesandbox.io/s/tqcfv0)

## [Demo](https://tqcfv0.csb.app/)

## Resource

- [Discord](https://discord.gg/Jwv7xaPRMS)
- [useEffect](https://reactjs.org/docs/hooks-effect.html)
- [Props](https://reactjs.org/docs/components-and-props.html)
- [useState](https://reactjs.org/docs/hooks-state.html)
- [onChange](https://sebhastian.com/react-onchange/)
