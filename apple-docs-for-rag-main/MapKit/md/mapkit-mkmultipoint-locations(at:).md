

- MapKit
- MKMultiPoint
-  locations(at:) 

Instance Method

# locations(at:)

Translates a point index set into a unit distance along the shape.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOS

``` source
func locations(at indexes: IndexSet) -> [CGFloat]
```

## Parameters 

`indexes`  

The index set of map points associated with the shape.

## Return Value

An array of CGFloat values.

## See Also

### Accessing the points in the shape

func points() -> UnsafeMutablePointer&lt;MKMapPoint>

Returns an array of map points associated with the shape.

var pointCount: Int

The number of points associated with the shape.

func location(atPointIndex: Int) -> CGFloat

Translates a point index into a unit distance along the shape.

