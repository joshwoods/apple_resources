

- MapKit
- MKMapRect
-  contains(\_:) 

Instance Method

# contains(\_:)

Returns a Boolean value that indicates whether the specified map point lies within the rectangle.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+watchOS 2.0+

``` source
func contains(_ point: MKMapPoint) -> Bool
```

## Parameters 

`point`  

The point to check.

## Return Value

true if the rectangle isn’t `null` or empty and the point is inside the rectangle; otherwise, false.

## Discussion

For this method, a point is inside the rectangle if its coordinates lie inside the rectangle or on the minimum X or minimum Y edge.

## See Also

### Intersecting the rectangle

func contains(MKMapRect) -> Bool

Returns a Boolean value that indicates whether one rectangle contains another.

func intersects(MKMapRect) -> Bool

Returns a Boolean value that indicates whether two rectangles intersect each other.

