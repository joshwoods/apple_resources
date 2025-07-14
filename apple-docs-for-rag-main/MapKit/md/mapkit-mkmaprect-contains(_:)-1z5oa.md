

- MapKit
- MKMapRect
-  contains(\_:) 

Instance Method

# contains(\_:)

Returns a Boolean value that indicates whether one rectangle contains another.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+watchOS 2.0+

``` source
func contains(_ rect2: MKMapRect) -> Bool
```

## Parameters 

`rect2`  

The rectangle that `rect1` might contain.

## Return Value

true if `rect2` is `null` or lies entirely inside `rect1`; otherwise, returns false if `rect1` is `null` or doesn’t completely enclose `rect2`.

## See Also

### Intersecting the rectangle

func contains(MKMapPoint) -> Bool

Returns a Boolean value that indicates whether the specified map point lies within the rectangle.

func intersects(MKMapRect) -> Bool

Returns a Boolean value that indicates whether two rectangles intersect each other.

