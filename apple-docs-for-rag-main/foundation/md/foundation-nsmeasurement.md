

- Foundation
-  NSMeasurement 

Class

# NSMeasurement

A numeric quantity labeled with a unit of measure, with support for unit conversion and unit-aware calculations.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class NSMeasurement
```

## Overview

Use this object in Swift when you need reference semantics or other Foundation-specific behavior.

An NSMeasurement object represents a quantity and unit of measure. The NSMeasurement class provides a programmatic interface to converting measurements into different units, as well as calculating the sum or difference between two measurements.

NSMeasurement objects are initialized with an Unit object and `double` value. NSMeasurement objects are immutable, and cannot be changed after being created.

You can use the MeasurementFormatter class to create localized string representations of NSMeasurement objects.

Important

The Swift overlay to the Foundation framework provides the Measurement structure, which bridges to the NSMeasurement class. For more information about value types, see Working with Cocoa Frameworks in Using Swift with Cocoa and Objective-C (Swift 4.1).

## Topics

### Creating Measurements

init(doubleValue: Double, unit: Unit)

Initializes a new measurement with a specified double-precision floating-point value and unit.

### Accessing Unit and Value

var unit: Unit

The unit of measure.

var doubleValue: Double

The measurement value, represented as a double-precision floating-point number.

### Converting to Other Units

func canBeConverted(to: Unit) -> Bool

Indicates whether the measurement can be converted to the given unit.

func converting(to: Unit) -> Measurement&lt;Unit>

Returns a measurement created by converting the receiver to the specified unit.

### Operating on Measurements

func adding(Measurement&lt;Unit>) -> Measurement&lt;Unit>

Returns a new measurement by adding the receiver to the specified measurement.

func subtracting(Measurement&lt;Unit>) -> Measurement&lt;Unit>

Returns a new measurement by subtracting the specified measurement from the receiver.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Essentials

struct Measurement

A numeric quantity labeled with a unit of measure, with support for unit conversion and unit-aware calculations.

class Unit

An abstract class representing a unit of measure.

class Dimension

An abstract class representing a dimensional unit of measure.

