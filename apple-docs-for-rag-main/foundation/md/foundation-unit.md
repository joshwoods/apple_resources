

- Foundation
-  Unit 

Class

# Unit

An abstract class representing a unit of measure.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class Unit
```

## Overview

Each instance of an Unit subclass consists of a symbol, which can be used to create string representations of NSMeasurement objects with the MeasurementFormatter class.

The Dimension subclass is an abstract class that represents a dimensional unit, which can be converted into different units of the same type. The Foundation framework provides several concrete Dimension subclasses to represent the most common physical quantities, including mass, length, duration, and speed.

### Subclassing Notes

Unit is intended for subclassing. For dimensional units, you should use one of the Apple provided Dimension subclasses listed in Table 1 of Dimension, or create a custom subclass of Dimension. You can create a direct subclass of Unit to represent a custom dimensionless unit, such as a count, score, or ratio.

## Topics

### Accessing Properties

var symbol: String

The symbolic representation of the unit.

### Creating Units

init(symbol: String)

Initializes a new unit with the specified symbol.

## Relationships

### Inherits From

- NSObject

### Inherited By

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

### Essentials

struct Measurement

A numeric quantity labeled with a unit of measure, with support for unit conversion and unit-aware calculations.

class NSMeasurement

A numeric quantity labeled with a unit of measure, with support for unit conversion and unit-aware calculations.

class Dimension

An abstract class representing a dimensional unit of measure.

