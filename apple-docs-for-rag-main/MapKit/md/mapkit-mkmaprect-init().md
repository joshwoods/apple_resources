

- MapKit
- MKMapRect
-  init() 

Initializer

# init()

Creates the rectangle with an empty region.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
init()
```

## Discussion

This method sets the origin point to `(0, 0)` and the size to `(0, 0)`.

## See Also

### Creating a map rectangle

init(origin: MKMapPoint, size: MKMapSize)

Creates the map rectangle with the specified point and size.

init(x: Double, y: Double, width: Double, height: Double)

Creates a new map rectangle structure from the specified values.

init(MKMapRect)

Returns the region that corresponds to the specified map rectangle.

