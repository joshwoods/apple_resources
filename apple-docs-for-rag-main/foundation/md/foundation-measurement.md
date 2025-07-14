

- Foundation
-  Measurement 

Structure

# Measurement

A numeric quantity labeled with a unit of measure, with support for unit conversion and unit-aware calculations.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
struct Measurement where UnitType : Unit
```

## Overview

A Measurement object represents a quantity and unit of measure. The Measurement type provides a programmatic interface to converting measurements into different units, as well as calculating the sum or difference between two measurements.

Measurement objects are initialized with a Unit object and double value. Measurement objects are immutable, and cannot be changed after being created.

Measurements support a large set of operators, including `+`, `-`, `*`, `/`, and a full set of comparison operators.

## Topics

### Creating a Measurement

init(value: Double, unit: UnitType)

Create a `Measurement` given a specified value and unit.

### Accessing the Value and Units

let unit: UnitType

The unit component of the measurement.

var value: Double

The value component of the measurement.

### Converting to Other Units

func convert(to: UnitType)

Converts the measurement to the specified unit.

func converted(to: UnitType) -> Measurement&lt;UnitType>

Returns a new measurement created by converting to the specified unit.

### Operating on a Measurement

static func * (Double, Measurement&lt;UnitType>) -> Measurement&lt;UnitType>

Multiply a scalar value by a measurement.

static func * (Measurement&lt;UnitType>, Double) -> Measurement&lt;UnitType>

Multiply a measurement by a scalar value.

static func + (Measurement&lt;UnitType>, Measurement&lt;UnitType>) -> Measurement&lt;UnitType>

Add two measurements.

static func + (Measurement&lt;UnitType>, Measurement&lt;UnitType>) -> Measurement&lt;UnitType>

Adds two measurements of the same dimension.

static func - (Measurement&lt;UnitType>, Measurement&lt;UnitType>) -> Measurement&lt;UnitType>

Subtract two measurements of the same Unit.

static func - (Measurement&lt;UnitType>, Measurement&lt;UnitType>) -> Measurement&lt;UnitType>

Subtract two measurements of the same Dimension.

static func / (Double, Measurement&lt;UnitType>) -> Measurement&lt;UnitType>

Divide a scalar value by a measurement.

static func / (Measurement&lt;UnitType>, Double) -> Measurement&lt;UnitType>

Divide a measurement by a scalar value.

### Formatting a Measurement

func formatted() -> String

Generates a locale-aware string representation of a measurement using the default measurement format style.

func formatted&lt;S>(S) -> S.FormatOutput

Generates a locale-aware string representation of a measurement using the provided measurement format style.

struct FormatStyle

A type that provides localized representations of measurements.

struct AttributedStyle

A type that provides localized representations of measurements with an attributed string.

### Comparing Measurements

static func > (Self, Self) -> Bool

Returns a Boolean value indicating whether the value of the first argument is greater than that of the second argument.

static func >= (Self, Self) -> Bool

Returns a Boolean value indicating whether the value of the first argument is greater than or equal to that of the second argument.

static func &lt; &lt;LeftHandSideType, RightHandSideType>(Measurement&lt;LeftHandSideType>, Measurement&lt;RightHandSideType>) -> Bool

Compare two measurements of the same `Unit`.

static func &lt;= (Self, Self) -> Bool

Returns a Boolean value indicating whether the value of the first argument is less than or equal to that of the second argument.

### Creating Ranges of Measurements

static func ... (Self) -> PartialRangeFrom&lt;Self>

Returns a partial range extending upward from a lower bound.

static func ... (Self) -> PartialRangeThrough&lt;Self>

Returns a partial range up to, and including, its upper bound.

static func ... (Self, Self) -> ClosedRange&lt;Self>

Returns a closed range that contains both of its bounds.

static func ..&lt; (Self, Self) -> Range&lt;Self>

Returns a half-open range that contains its lower bound but not its upper bound.

static func ..&lt; (Self) -> PartialRangeUpTo&lt;Self>

Returns a partial range up to, but not including, its upper bound.

### Using Reference Types

class NSMeasurement

A numeric quantity labeled with a unit of measure, with support for unit conversion and unit-aware calculations.

### Type Aliases

typealias Specification

typealias UnwrappedType

typealias ValueType

### Type Properties

static var defaultResolverSpecification: some ResolverSpecification

### Default Implementations

Comparable Implementations

Equatable Implementations

## Relationships

### Conforms To

- Comparable
- Copyable
- CustomDebugStringConvertible
- CustomReflectable
- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable
- ReferenceConvertible
- Sendable

## See Also

### Essentials

class NSMeasurement

A numeric quantity labeled with a unit of measure, with support for unit conversion and unit-aware calculations.

class Unit

An abstract class representing a unit of measure.

class Dimension

An abstract class representing a dimensional unit of measure.

