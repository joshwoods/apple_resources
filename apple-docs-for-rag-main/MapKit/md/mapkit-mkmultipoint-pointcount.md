

- MapKit
- MKMultiPoint
-  pointCount 

Instance Property

# pointCount

The number of points associated with the shape.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
var pointCount: Int { get }
```

## See Also

### Accessing the points in the shape

func points() -> UnsafeMutablePointer&lt;MKMapPoint>

Returns an array of map points associated with the shape.

func location(atPointIndex: Int) -> CGFloat

Translates a point index into a unit distance along the shape.

func locations(at: IndexSet) -> [CGFloat]

Translates a point index set into a unit distance along the shape.

