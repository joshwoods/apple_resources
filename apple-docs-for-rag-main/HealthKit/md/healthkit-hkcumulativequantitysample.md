

- HealthKit
-  HKCumulativeQuantitySample 

Class

# HKCumulativeQuantitySample

A sample that represents a cumulative quantity.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
class HKCumulativeQuantitySample
```

## Mentioned in 

Accessing condensed workout samples

## Overview

A quantity sample contains one or more HKQuantity objects. Each quantity represents a single piece of data with a single numeric value and the value’s associated units. Use these samples to store data that accumulates over time, such as step count, active energy burned, or walking distance.

The HKCumulativeQuantitySample class is a concrete subclass of the HKQuantitySample class. Cumulative quantity samples are immutable; you set the sample’s properties when you create it, and they cannot change.

### Extend Cumulative Quantity Samples

Like many HealthKit classes, you should not subclass the HKCumulativeQuantitySample class. You may extend this class by adding metadata with custom keys to save related data used by your app.

For more information, see init(type:quantity:start:end:metadata:).

## Topics

### Accessing Calculated Data

var sumQuantity: HKQuantity

The sum of all the quantities contained by the sample.

## Relationships

### Inherits From

- HKQuantitySample

### Inherited By

- HKCumulativeQuantitySeriesSample

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Basic samples

class HKDiscreteQuantitySample

A sample that represents a discrete quantity.

class HKQuantitySample

A sample that represents a quantity, including the value and the units.

class HKCategorySample

A sample with values from a short list of possible values.

class HKCorrelation

A sample that groups multiple related samples into a single entry.

Units and quantities

Objects used to specify a quantity for a given unit, and to convert between units.

Metadata Keys

Constants used to add metadata to objects stored in HealthKit.

