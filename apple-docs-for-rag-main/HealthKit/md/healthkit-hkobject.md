

- HealthKit
-  HKObject 

Class

# HKObject

A piece of data that can be stored inside the HealthKit store.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
class HKObject
```

## Mentioned in 

About the HealthKit framework

## Overview

The `HKObject` class is an abstract class. You should never instantiate a `HKObject` object directly. Instead, always work with one of its concrete subclasses: HKCategorySample, HKQuantitySample, HKCorrelation, or HKWorkout.

HealthKit objects are all immutable. With a few exceptions (such as the object’s source revision), the object’s properties are set when the object is first created and they cannot change.

## Topics

### Accessing Properties

var uuid: UUID

The universally unique identifier (UUID) for this HealthKit object.

var metadata: [String : Any]?

The metadata for this HealthKit object.

var device: HKDevice?

The device that generated the data for this object.

var sourceRevision: HKSourceRevision

The app or device that created this object.

var source: HKSource

A HealthKit source, representing the app or device that created this object.

Deprecated

### Specifying Predicate Key Paths

let HKPredicateKeyPathUUID: String

The key path for accessing the object’s UUID inside a predicate format string.

let HKPredicateKeyPathMetadata: String

The key path for accessing the object’s metadata dictionary inside a predicate format string.

## Relationships

### Inherits From

- NSObject

### Inherited By

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

### Abstract superclasses

class HKQuantitySample

A sample that represents a quantity, including the value and the units.

class HKSample

A HealthKit sample represents a piece of data associated with a start and end time.

