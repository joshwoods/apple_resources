

- Vision
- VNCircle
-  contains(\_:) 

Instance Method

# contains(\_:)

Determines if this circle, including its boundary, contains the specified point.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func contains(_ point: VNPoint) -> Bool
```

## Parameters 

`point`  

The point to test.

## Return Value

true if the point is contained within this circle, otherwise false.

## See Also

### Inspecting a Circle

var center: VNPoint

The circle’s center point.

var diameter: Double

The circle’s diameter.

var radius: Double

The circle’s radius.

func contains(VNPoint, inCircumferentialRingOfWidth: Double) -> Bool

Determines if a ring around this circle’s circumference contains the specified point.

