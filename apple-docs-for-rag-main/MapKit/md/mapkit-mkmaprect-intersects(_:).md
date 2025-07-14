

- MapKit
- MKMapRect
-  intersects(\_:) 

Instance Method

# intersects(\_:)

Returns a Boolean value that indicates whether two rectangles intersect each other.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+watchOS 2.0+

``` source
func intersects(_ rect2: MKMapRect) -> Bool
```

## Parameters 

`rect2`  

The second rectangle.

## Return Value

true if `rect1` and `rect2` intersect each other, or false if they don’t intersect or either rectangle is `null`.

## Discussion

The rectangles aren’t intersecting if the only intersection occurs along an edge. For a true intersection, the rectangles both need to enclose a single rectangular area with a width and height that are both greater than `0`.

## See Also

### Intersecting the rectangle

func contains(MKMapPoint) -> Bool

Returns a Boolean value that indicates whether the specified map point lies within the rectangle.

func contains(MKMapRect) -> Bool

Returns a Boolean value that indicates whether one rectangle contains another.

