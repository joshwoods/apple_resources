

- MapKit JS
- mapkit.MapRect
-  mapkit.MapRect 

Initializer

# mapkit.MapRect

Creates an object that represents a rectangular region of the map projection.

MapKit JS 5.0+

``` source
new mapkit.MapRect(
 number x,
 number y,
 number width,
 number height
);
```

## Parameters 

`x`  

The origin point along the east-west axis of the map projection.

`y`  

The origin point along the north-south axis of the map projection.

`width`  

The distance, in map units, along the east-west axis of the map projection.

`height`  

The distance, in map units, along the north-south axis of the map projection.

## Discussion

The following example demonstrates how to create a `mapkit.MapRect` instance from map units and inspect the object’s `origin` and `size` properties:

```
// Defining a MapRect (x, y, width, height):
var mapRect = new mapkit.MapRect(0.1, 0.2, 0.3, 0.4);

// mapRect.origin is a MapPoint:
var x = mapRect.origin.x; // 0.1
var y = mapRect.origin.x; // 0.2

// mapRect.size is a MapSize:
var width = mapRect.size.width; // 0.3
var height = mapRect.size.height; // 0.4
```

