<!-- Generated by documentation.js. Update this documentation by updating the source code. -->

### Table of Contents

-   [togglePerspective][1]
-   [fitBounds][2]
-   [updateMap][3]
-   [toggleSplitMap][4]

## togglePerspective

Toggle between 3d and 2d map.
param {void}

## fitBounds

Fit current map ti a new bounds
param {Array} - bounds: `[lngMin, latMin, lngMax, latMax]`

**Examples**

```javascript
this.props.dispatch(fitBounds([-122.23, 37.127, -122.11, 37.456]))
```

## updateMap

Update map viewport

**Parameters**

-   `viewport` **[Object][5]** viewport object container one or any of these properties `width`, `height`, `latitude` `longitude`, `zoom`, `pitch`, `bearing`, `dragRotate`
    -   `viewport.width` **[Number][6]** Width of viewport
    -   `viewport.height` **[Number][6]** Height of viewport
    -   `viewport.zoom` **[Number][6]** Zoom of viewport
    -   `viewport.pitch` **[Number][6]** Camera angle in degrees (0 is straight down)
    -   `viewport.bearing` **[Number][6]** Map rotation in degrees (0 means north is up)
    -   `viewport.latitude` **[Number][6]** Latitude center of viewport on map in mercator projection
    -   `viewport.longitude` **[Number][6]** Longitude Center of viewport on map in mercator projection
    -   `viewport.dragRotate` **[Boolean][7]** Whether to enable drag and rotate map into perspective viewport

**Examples**

```javascript
this.props.dispatch(updateMap({latitude: 37.75043, longitude: -122.34679, width: 800, height: 1200}))
```

## toggleSplitMap

Toggle between one or split maps
param {void}

[1]: #toggleperspective

[2]: #fitbounds

[3]: #updatemap

[4]: #togglesplitmap

[5]: https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Object

[6]: https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Number

[7]: https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Boolean