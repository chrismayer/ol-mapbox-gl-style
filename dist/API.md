# getStyleFunction

Creates a style function from the `glStyle` object for all layers that use
the specified `source`, which needs to be a `"type": "vector"`
source.

**Parameters**

-   `glStyle` **([string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) \| [Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object))** Mapbox GL style object.
-   `source` **[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** `source` key from the Mapbox GL style object.
-   `resolutions` **[Array](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array)&lt;[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)>** Resolutions for mapping resolution to
    zoom level. For tile layers, this can be
    `layer.getSource().getTileGrid().getResolutions()`.

Returns **ol.style.StyleFunction** Style function for use in
`ol.layer.Vector` or `ol.layer.VectorTile`.
