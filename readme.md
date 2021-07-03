# Radix colors for Tailwind

This adds the (radix colour palette)[https://www.radix-ui.com/colors] to Tailwind CSS

You can add this plugin under the `plugins` key of your `tailwind.config.js` as follows:

```json
plugins: [
    require("radix-colors-for-tailwind")({
      colors: ["blue", "cyan", "lime"],
    }),
],
```

Replace the colours in the `colors` array with whatever colours you want including
