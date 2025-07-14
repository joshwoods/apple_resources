

- MapKit JS
- mapkit.MapPoint
-  mapkit.MapPoint 

Initializer

# mapkit.MapPoint

Creates a map location.

MapKit JS 5.0+

``` source
new mapkit.MapPoint(
 number x,
 number y
);
```

## Parameters 

`x`  

The point along the east-west axis of the map projection.

`y`  

The point along the north-south axis of the map projection.

## Discussion

The x and y values of the point are unit values. MapKit JS expects the value to be between `0` and `1,` and represents an interpolated location on the map projection in the x and y coordinates, respectively.

The following example creates a point that’s one-tenth across the map projection along the x-axis, and half way across the y-axis:

```
var mapPoint = new mapkit.MapPoint(0.1, 0.5);
var x = mapPoint.x; // 0.1
var y = mapPoint.y; // 0.5
```

