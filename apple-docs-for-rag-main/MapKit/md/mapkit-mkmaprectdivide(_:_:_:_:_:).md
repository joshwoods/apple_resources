

- MapKit
-  MKMapRectDivide(\_:\_:\_:\_:\_:) 

Function

# MKMapRectDivide(\_:\_:\_:\_:\_:)

Divides the specified rectangle into two smaller rectangles.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+watchOS 2.0+

``` source
func MKMapRectDivide(
    _ rect: MKMapRect,
    _ slice: UnsafeMutablePointer,
    _ remainder: UnsafeMutablePointer,
    _ amount: Double,
    _ edge: CGRectEdge
)
```

## Parameters 

`rect`  

The rectangle to divide.

`slice`  

On input, a pointer to a map rectangle. On output, this parameter contains the portion of `rect` that the method removes.

`remainder`  

On input, a pointer to a map rectangle. On output, this parameter contains the remaining portion of `rect` that the method doesn’t remove.

`amount`  

The amount of `rect` to remove along the specified edge. If this value is negative, the system sets it to `0`.

`edge`  

The edge from which to remove the specified amount.

## See Also

### Modifying the rectangle

func union(MKMapRect) -> MKMapRect

Returns a rectangle that represents the union of two rectangles.

func intersection(MKMapRect) -> MKMapRect

Returns the rectangle that represents the intersection of two rectangles.

func insetBy(dx: Double, dy: Double) -> MKMapRect

Returns the specified rectangle with an inset by the specified amounts.

func offsetBy(dx: Double, dy: Double) -> MKMapRect

Returns a rectangle with an origin point that shifts by the specified amount.

