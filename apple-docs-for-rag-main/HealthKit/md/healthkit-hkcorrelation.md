

- HealthKit
-  HKCorrelation 

Class

# HKCorrelation

A sample that groups multiple related samples into a single entry.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
class HKCorrelation
```

## Mentioned in 

Saving data to HealthKit

About the HealthKit framework

## Overview

HealthKit uses correlations to represent both blood pressure and food.

- Blood pressure correlations always include two quantity samples, representing the systolic and diastolic values.

- Food correlations can contain a wide range of dietary information about the food, including information about the fat, protein, carbohydrates, energy, and vitamins consumed.

In general, a food correlation should include at least a dietaryEnergyConsumed sample. You can also add nutritional quantity samples for any other items you want to track. Use the HKMetadataKeyFoodType key to indicate the food’s name.

The HKCorrelation class is a concrete subclass of the HKSample class. Correlations are immutable: You set the correlation’s properties when the object is first created, and they cannot change.

### Extend Correlation Samples

Like many HealthKit classes, the `HKCorrelation` class should not be subclassed. You can extend the correlation class by adding metadata with custom keys as appropriate for your app.

For more information, see the init(type:start:end:objects:metadata:) method.

## Topics

### Creating Correlations

convenience init(type: HKCorrelationType, start: Date, end: Date, objects: Set&lt;HKSample>)

Instantiates and returns a new correlation instance.

convenience init(type: HKCorrelationType, start: Date, end: Date, objects: Set&lt;HKSample>, metadata: [String : Any]?)

Instantiates and returns a new correlation instance with the provided metadata.

convenience init(type: HKCorrelationType, start: Date, end: Date, objects: Set&lt;HKSample>, device: HKDevice?, metadata: [String : Any]?)

Instantiates and returns a new correlation instance with the provided device and metadata.

### Getting Correlation Data

var correlationType: HKCorrelationType

The type for this correlation.

var objects: Set&lt;HKSample>

The set of sample objects that make up the correlation.

func objects(for: HKObjectType) -> Set&lt;HKSample>

Returns a set containing all the objects of the specified type in the correlation.

### Specifying Predicate Key Paths

let HKPredicateKeyPathCorrelation: String

The key path for accessing the object’s correlation inside a predicate format string.

## Relationships

### Inherits From

- HKSample

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

class HKQuantitySample

A sample that represents a quantity, including the value and the units.

class HKCategorySample

A sample with values from a short list of possible values.

Units and quantities

Objects used to specify a quantity for a given unit, and to convert between units.

Metadata Keys

Constants used to add metadata to objects stored in HealthKit.

