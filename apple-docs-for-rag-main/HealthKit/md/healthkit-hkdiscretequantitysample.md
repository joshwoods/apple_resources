

- HealthKit
-  HKDiscreteQuantitySample 

Class

# HKDiscreteQuantitySample

A sample that represents a discrete quantity.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
class HKDiscreteQuantitySample
```

## Mentioned in 

Accessing condensed workout samples

## Overview

A quantity sample contains one or more HKQuantity objects. Each quantity represents a single piece of data with a single numeric value and the value’s associated units. Use these samples to store data representing independent measurements, such as height, heart rate, or temperature.

The HKDiscreteQuantitySample class is a concrete subclass of the HKQuantitySample class. Discrete quantity samples are immutable; you set the sample’s properties when you create it, and they cannot change.

### Extend Discrete Quantity Samples

Like many HealthKit classes, you should not subclass the HKDiscreteQuantitySample class. You may extend this class by adding metadata with custom keys to save related data used by your app.

For more information, see init(type:quantity:start:end:metadata:).

## Topics

### Accessing Calculated Values

var averageQuantity: HKQuantity

The average of all quantities contained by the sample.

var maximumQuantity: HKQuantity

The maximum quantity contained by the sample.

var minimumQuantity: HKQuantity

The minimum value contained by the sample.

var mostRecentQuantity: HKQuantity

The most recent quantity contained by the sample.

var mostRecentQuantityDateInterval: DateInterval

The date interval for the most recent quantity contained by the sample.

### Specifying Predicate Key Paths

let HKPredicateKeyPathMin: String

The key path for the sample’s minimum quantity.

let HKPredicateKeyPathAverage: String

The key path for the sample’s average quantity.

let HKPredicateKeyPathMax: String

The key path for the sample’s maximum quantity.

let HKPredicateKeyPathMostRecent: String

The key path for the sample’s most recent quantity.

let HKPredicateKeyPathMostRecentStartDate: String

The key path for the start date of the sample’s most recent quantity.

let HKPredicateKeyPathMostRecentEndDate: String

The key path for the end date of the sample’s most recent quantity.

let HKPredicateKeyPathMostRecentDuration: String

A key path for the duration of the sample’s most recent quantity.

## Relationships

### Inherits From

- HKQuantitySample

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

class HKCumulativeQuantitySample

A sample that represents a cumulative quantity.

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

