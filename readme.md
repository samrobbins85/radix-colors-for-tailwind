# Radix colors for Tailwind

This adds the [radix color palette](https://www.radix-ui.com/colors) to Tailwind CSS

You can add this plugin under the `plugins` key of your `tailwind.config.js` as follows:

```js
plugins: [
    require("radix-colors-for-tailwind")({
      colors: ["blue", "cyan", "lime"],
    }),
],
```

Replace the colours in the `colors` array with whatever colours you want including

## Additional features

This package also includes a range of component classes to speed up development, these are based on the suggestions for how to use [the scale](https://www.radix-ui.com/docs/colors/palette-composition/understanding-the-scale)

### `color-bg`

If you do `color-bg` e.g. `blue-bg`, you will get a background color of step `3`, this follows the pattern explained [here](https://www.radix-ui.com/docs/colors/palette-composition/understanding-the-scale#steps-35-component-backgrounds). If you want to make this interactive, instead use the class `color-bg-int`, and you will also have states for hover and focus.

### `color-cta`

Following a similar pattern, `color-cta` will give you a background color of step `4` for a darker look, and similarly gives you the option of `color-cta-int` to have hover and focus states

### `color-border`

If you want to add borders to your components, you can use the `color-border` pattern, this uses step `6` by default, but will use step `7` if you do `color-border-int`

### `color-solid`

If you want solid backgrounds to your components rather than the lighter ones provided by the other classes, then you can use `color-solid`, giving you a background of step `9`, again, there's a `color-solid-int` option that also gives you a hover state at step `10`
