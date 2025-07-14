

- MapKit
- MKMapRect
-  offsetBy(dx:dy:) 

Instance Method

# offsetBy(dx:dy:)

Returns a rectangle with an origin point that shifts by the specified amount.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+watchOS 2.0+

``` source
func offsetBy(
    dx: Double,
    dy: Double
) -> MKMapRect
```

## Parameters 

`dx`  

The amount (in map points) to shift the x-coordinate of the origin point.

`dy`  

The amount (in map points) to shift the x-coordinate of the origin point.

## Return Value

The offset rectangle. If the original rectangle is `null`, that rectangle returns instead.

## See Also

### Modifying the rectangle

func union(MKMapRect) -> MKMapRect

Returns a rectangle that represents the union of two rectangles.

func intersection(MKMapRect) -> MKMapRect

Returns the rectangle that represents the intersection of two rectangles.

func insetBy(dx: Double, dy: Double) -> MKMapRect

Returns the specified rectangle with an inset by the specified amounts.

func MKMapRectDivide(MKMapRect, UnsafeMutablePointer&lt;MKMapRect>, UnsafeMutablePointer&lt;MKMapRect>, Double, CGRectEdge)

Divides the specified rectangle into two smaller rectangles.

