# BBox Date Line

Modifies a BBox to fit within the bounds of the International Date Line.

## API

<!-- Generated by documentation.js. Update this documentation by updating the source code. -->

#### Table of Contents

-   [bbox](#bbox)
-   [center](#center)
-   [latitude](#latitude)
-   [longitude](#longitude)

### bbox

Modifies a BBox to fit within the bounds of the International Date Line.

**Parameters**

-   `bbox` **(BBox | FeatureCollection | Feature&lt;any>)** BBox [west, south, east, north] or GeoJSON Feature

**Examples**

```javascript
dateline.bbox([190, 100, -200, -120])
//= [-170, -80, 160, 60]
```

Returns **BBox** valid BBox extent

### center

Modifies a Center to fit within the bounds of the International Date Line.

**Parameters**

-   `center` **(\[[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number), [number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)] | BBox | FeatureCollection | Feature&lt;any>)** Center [lng, lat], BBox [west, south, east, south] or GeoJSON Feature

**Examples**

```javascript
dateline.center([190, 100])
//= [-170, -80]
```

Returns **\[[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number), [number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)]** valid center coordinate

### latitude

Modifies a Latitude to fit within +/-90 degrees.

**Parameters**

-   `lat` **[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)** latitude to modify

**Examples**

```javascript
dateline.latitude(100)
//= -80
```

Returns **[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)** modified latitude

### longitude

Modifies a Longitude to fit within +/-180 degrees.

**Parameters**

-   `lng` **[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)** longitude to modify

**Examples**

```javascript
dateline.longitude(190)
//= -170
```

Returns **[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)** modified longitude