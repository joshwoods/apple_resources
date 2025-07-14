

- MapKit
- MKMapRect
-  init(x:y:width:height:) 

Initializer

# init(x:y:width:height:)

Creates a new map rectangle structure from the specified values.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
init(
    x: Double,
    y: Double,
    width: Double,
    height: Double
)
```

## Parameters 

`x`  

The point along the east-west axis of the map projection to use for the origin.

`y`  

The point along the north-south axis of the map projection to use for the origin.

`width`  

The width of the rectangle (measured using map points).

`height`  

The height of the rectangle (measured using map points).

## Return Value

A map rectangle with the specified values.

## See Also

### Creating a map rectangle

init()

Creates the rectangle with an empty region.

init(origin: MKMapPoint, size: MKMapSize)

Creates the map rectangle with the specified point and size.

init(MKMapRect)

Returns the region that corresponds to the specified map rectangle.

