

- MapKit
- MKCircle
-  init(mapRect:) 

Initializer

# init(mapRect:)

Creates and returns a circle object that derives the circular area from the specified rectangle.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
convenience init(mapRect: MKMapRect)
```

## Parameters 

`mapRect`  

The map rectangle that determines the circular area. The initializer uses the center point of the rectangle as the center point of the circle. If the rectangle isn’t a square, the method uses the longest side of the rectangle to define the radius of the resulting circle.

## Return Value

A circle overlay object.

## See Also

### Creating a circle overlay

convenience init(center: CLLocationCoordinate2D, radius: CLLocationDistance)

Creates and returns a circle object using the specified coordinate and radius.

