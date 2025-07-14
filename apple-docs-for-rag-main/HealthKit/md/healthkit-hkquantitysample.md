

- HealthKit
-  HKQuantitySample 

Class

# HKQuantitySample

A sample that represents a quantity, including the value and the units.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
class HKQuantitySample
```

## Mentioned in 

About the HealthKit framework

Accessing condensed workout samples

Saving data to HealthKit

## Overview

A quantity sample contains one or more HKQuantity objects. Each quantity represents a single piece of data with a single numeric value and the value’s associated units. For example, you can use quantity samples to record the user’s height, the user’s current heart rate, or the number of calories in a hamburger. HealthKit provides a wide range of quantity types, letting you track many different health and fitness features.

The HKQuantitySample class is a subclass of the HKSample class. Quantity samples are immutable; you set the sample’s properties when you create it, and they cannot change.

In iOS 13 and later and watchOS 6 and later, HKQuantitySample is an abstract superclass for the HKCumulativeQuantitySample and HKDiscreteQuantitySample concrete subclasses. The system automatically selects the correct subclass based on the HKQuantityType object used to create the sample.

### Extend Quantity Samples

Like many HealthKit classes, you should not subclass the HKQuantitySample class. You may extend this class by adding metadata with custom keys to save related data used by your app.

For more information, see init(type:quantity:start:end:metadata:).

## Topics

### Creating Quantity Samples

convenience init(type: HKQuantityType, quantity: HKQuantity, start: Date, end: Date)

Returns a sample containing a numeric measurement.

convenience init(type: HKQuantityType, quantity: HKQuantity, start: Date, end: Date, metadata: [String : Any]?)

Returns a sample containing a numeric measurement with the provided metadata.

convenience init(type: HKQuantityType, quantity: HKQuantity, start: Date, end: Date, device: HKDevice?, metadata: [String : Any]?)

Returns a sample containing a numeric measurement with the provided device and metadata.

### Getting Property Data

var quantity: HKQuantity

The quantity for this sample.

var count: Int

The number of quantities contained in this sample.

var quantityType: HKQuantityType

The quantity type for this sample.

### Specifying Predicate Key Paths

let HKPredicateKeyPathQuantity: String

The key path for accessing the sample’s quantity.

let HKPredicateKeyPathCount: String

A key path for the sample’s count.

## Relationships

### Inherits From

- HKSample

### Inherited By

- HKCumulativeQuantitySample
- HKDiscreteQuantitySample

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

class HKDiscreteQuantitySample

A sample that represents a discrete quantity.

class HKCategorySample

A sample with values from a short list of possible values.

class HKCorrelation

A sample that groups multiple related samples into a single entry.

Units and quantities

Objects used to specify a quantity for a given unit, and to convert between units.

Metadata Keys

Constants used to add metadata to objects stored in HealthKit.

