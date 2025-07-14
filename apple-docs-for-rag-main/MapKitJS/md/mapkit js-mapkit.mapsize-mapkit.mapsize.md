

- MapKit JS
- mapkit.MapSize
-  mapkit.MapSize 

Initializer

# mapkit.MapSize

Creates an object containing the width and height of a projected coordinate span.

MapKit JS 5.0+

``` source
new mapkit.MapSize(
 number width,
 number height
);
```

## Parameters 

`width`  

The distance in map units along the east-west axis of the map projection.

`height`  

The distance in map units along the north-south axis of the map projection.

## Discussion

The following example demonstrates how to create a `mapkit.MapSize` instance from map units:

```
var mapSize = new mapkit.MapSize(0.3, 0.4);
var width = mapSize.width; // 0.3
var height = mapSize.height; // 0.4
```

