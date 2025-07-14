

- MapKit
- MKMultiPoint
-  location(atPointIndex:) 

Instance Method

# location(atPointIndex:)

Translates a point index into a unit distance along the shape.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func location(atPointIndex index: Int) -> CGFloat
```

## Parameters 

`index`  

The index of the map point associated with the shape.

## Return Value

A CGFloat value that indicates the unit distance along the shape.

## See Also

### Accessing the points in the shape

func points() -> UnsafeMutablePointer&lt;MKMapPoint>

Returns an array of map points associated with the shape.

var pointCount: Int

The number of points associated with the shape.

func locations(at: IndexSet) -> [CGFloat]

Translates a point index set into a unit distance along the shape.

