

- Foundation
-  UnitElectricPotentialDifference 

Class

# UnitElectricPotentialDifference

A unit of measure for electric potential difference.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class UnitElectricPotentialDifference
```

## Overview

You typically use instances of UnitElectricPotentialDifference to represent specific quantities of electric potential difference using the NSMeasurement class.

### Electric Potential Difference

Electric potential difference is the amount of electric potential energy of a point charge at a point in space. The SI unit for electric potential difference is the volt (V), which is derived as the difference in electric potential energy between two points of a linear conductor when an electric current of one ampere dissipates one watt of power between those points (1V = 1W/1A).

The UnitElectricPotentialDifference class defines its baseUnit() as volts, and provides the following units, which are initialized using UnitConverterLinear converters with the specified coefficients:

| Name | Method | Symbol | Coefficient |
|----|----|----|----|
| Megavolts | megavolts | MV | `1000000.0` |
| Kilovolts | kilovolts | kV | `1000.0` |
| Volts | volts | V | `1.0` |
| Millivolts | millivolts | mV | `0.001` |
| Microvolts | microvolts | µV | `0.000001` |

## Topics

### Accessing the Base Unit

class func baseUnit() -> Self

Returns the base unit.

### Accessing Predefined Units

class var megavolts: UnitElectricPotentialDifference

The megavolts unit of electric potential difference.

class var kilovolts: UnitElectricPotentialDifference

The kilovolts unit of electric potential difference.

class var volts: UnitElectricPotentialDifference

The volts unit of electric potential difference.

class var millivolts: UnitElectricPotentialDifference

The millivolts unit of electric potential difference.

class var microvolts: UnitElectricPotentialDifference

The microvolts unit of electric potential difference.

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

### Electricity

class UnitElectricCharge

A unit of measure for electric charge.

class UnitElectricCurrent

A unit of measure for electric current.

class UnitElectricResistance

A unit of measure for electric resistance.

