# Simulated Devices

`devices.json` is a catalog of common web-enabled devices and their properties.

    {
      TYPES: [ "phones", … ],
      phones: [
        {
          name: "LePhone",
          width: 360,
          height: 640,
          pixelRatio: 3,
          userAgent: "Mozilla/5.0 (Mobile; rv:39.0) Gecko/39.0 Firefox/39.0",
          featured: true,
          touch: true
        }
      ], …
    }

## Device properties

- `name` brand and model(s).
- `width` viewport width.
- `height` viewport height.
- `pixelRatio` ratio from viewport to physical screen pixels.
- `userAgent` UA string of the device's browser.
- `touch` whether it has a touch screen.
- `os` the OS type it usually ships with.
- `featured` if set to true, the device appears in the RDM drop down list (Firefox UI) by default

## Device types

- `phones` (smart phones)
- `tablets`
- `laptops`
- `televisions`
- `consoles` (gaming consoles)
- `watches` (smart watches)

## Downloads

- Stable: [Mozilla CDN](https://code.cdn.mozilla.net/devices/devices.json).
- Latest: [GitHub](https://raw.githubusercontent.com/mozilla/simulated-devices/master/devices.json).

## Contribute

- Use the `check.html` helper.
- Use `node test.js` to verify your `devices.json`.
- Submit [pull requests](https://github.com/jankeromnes/devices/pulls).

## Sources

- Chrome Devtools: [emulated_devices/module.json](https://source.chromium.org/chromium/chromium/src/+/master:third_party/devtools-frontend/src/front_end/emulated_devices/module.json).
- Wikipedia: [Comparison of Firefox OS devices](https://en.wikipedia.org/wiki/Comparison_of_Firefox_OS_devices).
- MDN: [Firefox OS compatible devices](https://developer.mozilla.org/en-US/Firefox_OS/Firefox_OS_build_prerequisites).
- My Tesla Motors: [Model S Web Browser Capabilities](http://my.teslamotors.com/fr_CA/forum/forums/tesla-model-s-web-browser-capabilities).
- Various other online sources.
