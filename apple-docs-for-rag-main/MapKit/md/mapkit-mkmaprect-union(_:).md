

- MapKit
- MKMapRect
-  union(\_:) 

Instance Method

# union(\_:)

Returns a rectangle that represents the union of two rectangles.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+watchOS 2.0+

``` source
func union(_ rect2: MKMapRect) -> MKMapRect
```

## Parameters 

`rect2`  

The second rectangle.

## Return Value

A rectangle with an area that encompasses the two rectangles and the space between them.

## Discussion

If either rectangle is `null`, this method returns the other rectangle. This method sets the origin point of the returned rectangle to the smaller of the x and y values for the two rectangles. Similarly, the method computes the size and width of the rectangle by taking the maximum x and y values and subtracting the x and y values for the new origin point.

## See Also

### Modifying the rectangle

func intersection(MKMapRect) -> MKMapRect

Returns the rectangle that represents the intersection of two rectangles.

func insetBy(dx: Double, dy: Double) -> MKMapRect

Returns the specified rectangle with an inset by the specified amounts.

func offsetBy(dx: Double, dy: Double) -> MKMapRect

Returns a rectangle with an origin point that shifts by the specified amount.

func MKMapRectDivide(MKMapRect, UnsafeMutablePointer&lt;MKMapRect>, UnsafeMutablePointer&lt;MKMapRect>, Double, CGRectEdge)

Divides the specified rectangle into two smaller rectangles.

