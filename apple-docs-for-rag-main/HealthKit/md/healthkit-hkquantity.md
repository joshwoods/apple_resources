

- HealthKit
-  HKQuantity 

Class

# HKQuantity

An object that stores a value for a given unit.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
class HKQuantity
```

## Mentioned in 

Defining and converting units and quantities

Saving data to HealthKit

## Overview

HealthKit uses quantity objects to store numerical data. When you create a quantity, you provide both the quantity’s value and unit.

Quantities are immutable objects: Their values are set when the object is first created and cannot change.

### Converting Units

You can request the value from a quantity object in any compatible units. For example, if you create a length quantity in feet, you can then request the length in meters. The quantity object automatically converts its value to the requested units.

### Using Quantities

Like many HealthKit classes, the HKQuantity class is not extendible and should not be subclassed. To help promote sharing data between apps, HKQuantity objects use only the units defined by the HKUnit class.

## Topics

### Creating Quantities

convenience init(unit: HKUnit, doubleValue: Double)

Instantiates and returns a new quantity object.

### Working With Units

func `is`(compatibleWith: HKUnit) -> Bool

Returns a boolean value indicating whether the quantity is compatible with the provided unit.

func doubleValue(for: HKUnit) -> Double

Returns the quantity’s value in the provided unit.

### Comparing Quantities

func compare(HKQuantity) -> ComparisonResult

Compares two values after converting them to the same units.

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
- Sendable

## See Also

### Units and quantities

Defining and converting units and quantities

Create and convert units and quantities.

class HKUnit

A class for managing the units of measure within HealthKit.

enum HKMetricPrefix

Prefixes that can be added to SI units to change the order of magnitude.

