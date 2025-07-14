

- MapKit
- MKMapRect
-  intersection(\_:) 

Instance Method

# intersection(\_:)

Returns the rectangle that represents the intersection of two rectangles.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+watchOS 2.0+

``` source
func intersection(_ rect2: MKMapRect) -> MKMapRect
```

## Parameters 

`rect2`  

The second rectangle.

## Return Value

The rectangle representing the intersection of the two rectangles, or null if there’s no intersection.

## See Also

### Modifying the rectangle

func union(MKMapRect) -> MKMapRect

Returns a rectangle that represents the union of two rectangles.

func insetBy(dx: Double, dy: Double) -> MKMapRect

Returns the specified rectangle with an inset by the specified amounts.

func offsetBy(dx: Double, dy: Double) -> MKMapRect

Returns a rectangle with an origin point that shifts by the specified amount.

func MKMapRectDivide(MKMapRect, UnsafeMutablePointer&lt;MKMapRect>, UnsafeMutablePointer&lt;MKMapRect>, Double, CGRectEdge)

Divides the specified rectangle into two smaller rectangles.

