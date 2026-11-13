# TransparentXImages

**[Open the app](https://05v.github.io/TransparentXImages/)** · free, runs in your browser, your image is never uploaded.

Turn any image into a white, transparent PNG that looks right on X's black background.

![TransparentXImages demo: dropping a photo, tuning contrast and switching the preview background](docs/demo.gif)

## Why

X shows transparent images on black. A normal photo or logo with transparency can disappear into that background. This tool turns your image into white with transparency, so it shows up as clean white artwork on black.

## How it works

Each pixel's brightness becomes its opacity. Bright areas turn solid white, dark areas fade to transparent.

- **Contrast** and **Brightness** shape that curve before it is applied.
- **Max opacity** caps how solid the brightest parts get.
- **Invert** flips it, for a dark subject on a light background.
- Areas that are already transparent in your image stay transparent.

The preview runs on a downscaled copy so the sliders stay smooth on large photos. The download is made from the full-size original.

## Use it

1. [Open the app](https://05v.github.io/TransparentXImages/).
2. Drop an image, click to choose one, or paste with Cmd + V (Ctrl + V on Windows).
3. Adjust the sliders and check the result on black or on the transparency grid.
4. Click **Download PNG**.

## Run locally

It's a single HTML file with no dependencies and no build step.

```bash
git clone https://github.com/05v/TransparentXImages.git
cd TransparentXImages
open index.html
```

## Built with

HTML, CSS and plain JavaScript, using the Canvas 2D API.

## License

[MIT](LICENSE)
