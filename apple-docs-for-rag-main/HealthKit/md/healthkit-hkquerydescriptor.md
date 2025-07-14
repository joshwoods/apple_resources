

- HealthKit
-  HKQueryDescriptor 

Class

# HKQueryDescriptor

A descriptor that specifies a set of samples based on the data type and a predicate.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 13.0+visionOS 1.0+watchOS 8.0+

``` source
class HKQueryDescriptor
```

## Overview

Use descriptors to create queries that return multiple data types. You can use descriptors when creating HKSampleQuery, HKAnchoredObjectQuery, or HKObserverQuery instances.

## Topics

### Creating Query Descriptors

init(sampleType: HKSampleType, predicate: NSPredicate?)

Creates a new descriptor for the data type and predicate you provided.

### Accessing Descriptor Data

var predicate: NSPredicate?

The predicate that filters samples matching this descriptor.

var sampleType: HKSampleType

The data type of samples that match this descriptor.

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

### Basic queries

struct HKSampleQueryDescriptor

A query interface that reads samples using Swift concurrency.

class HKSampleQuery

A general query that returns a snapshot of all the matching samples currently saved in the HealthKit store.

class HKCorrelationQuery

A query that performs complex searches based on the correlation’s contents, and returns a snapshot of all matching samples.

class HKQuery

An abstract class for all the query classes in HealthKit.

