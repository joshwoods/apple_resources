

- Vision
- VNCircle
-  radius 

Instance Property

# radius

The circle’s radius.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var radius: Double { get }
```

## See Also

### Inspecting a Circle

var center: VNPoint

The circle’s center point.

var diameter: Double

The circle’s diameter.

func contains(VNPoint) -> Bool

Determines if this circle, including its boundary, contains the specified point.

func contains(VNPoint, inCircumferentialRingOfWidth: Double) -> Bool

Determines if a ring around this circle’s circumference contains the specified point.

