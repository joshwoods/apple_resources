

- Foundation
-  UnitAngle 

Class

# UnitAngle

A unit of measure for planar angle and rotation.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class UnitAngle
```

## Overview

You typically use instances of UnitAngle to represent specific quantities of planar angle using the NSMeasurement class.

### Angle

Angle is a quantity of rotation. The SI unit for angle is the radian (rad), which is dimensionless and defined to be the angle subtended by an arc that is equal in length to the radius of a circle. Angle is also commonly expressed in terms of degrees (°) and revolutions (rev).

The UnitAngle class defines its baseUnit() as degrees, and provides the following units, which are initialized using UnitConverterLinear converters with the specified coefficients:

| Name | Method | Symbol | Definition |
|----|----|----|----|
| Degrees | degrees | ° | `1.0` |
| Arc Minutes | arcMinutes | ʹ | `0.016667` |
| Arc Seconds | arcSeconds | ʺ | `0.00027778` |
| Radians | radians | rad | `57.2958` |
| Gradians | gradians | grad | `0.9` |
| Revolutions | revolutions | rev | `360` |

## Topics

### Accessing the Base Unit

class func baseUnit() -> Self

Returns the base unit.

### Accessing Predefined Units

class var degrees: UnitAngle

The degrees unit of angle.

class var arcMinutes: UnitAngle

The arc minutes unit of angle.

class var arcSeconds: UnitAngle

The arc seconds unit of angle.

class var radians: UnitAngle

The radians unit of angle.

class var gradians: UnitAngle

The gradians unit of angle.

class var revolutions: UnitAngle

The revolutions unit of angle.

## Relationships

### Inherits From

- Dimension

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
- Sendable

## See Also

### Physical Dimension

class UnitArea

A unit of measure for area.

class UnitLength

A unit of measure for length.

class UnitVolume

A unit of measure for volume.

