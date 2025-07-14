

- Vision
-  VNCircle 

Class

# VNCircle

An immutable 2D circle represented by its center point and radius.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class VNCircle
```

## Topics

### Creating a Circle

init(center: VNPoint, radius: Double)

Creates a circle with the specified center and radius.

convenience init(center: VNPoint, diameter: Double)

Creates a circle with the specified center and diameter.

class var zero: VNCircle

A circle object centered at the origin, with a radius of zero.

### Inspecting a Circle

var center: VNPoint

The circle’s center point.

var diameter: Double

The circle’s diameter.

var radius: Double

The circle’s radius.

func contains(VNPoint) -> Bool

Determines if this circle, including its boundary, contains the specified point.

func contains(VNPoint, inCircumferentialRingOfWidth: Double) -> Bool

Determines if a ring around this circle’s circumference contains the specified point.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Common data types

class VNVector

An immutable 2D vector represented by its x-axis and y-axis projections.

