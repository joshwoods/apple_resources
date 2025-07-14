

- HealthKit
-  HKSourceQuery 

Class

# HKSourceQuery

A query that returns a list of sources, such as apps and devices, that have saved matching queries to the HealthKit store.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
class HKSourceQuery
```

## Overview

Source queries return a list of sources that have saved samples matching the specified sample types. Sources can be apps or devices (like Apple Watch or Bluetooth heart-rate monitors).

Source queries are immutable: Their properties are set when they are first created, and they can’t change.

## Topics

### Creating Source Queries

Executing Source Queries

Create and run source queries.

init(sampleType: HKSampleType, samplePredicate: NSPredicate?, completionHandler: (HKSourceQuery, Set&lt;HKSource>?, (any Error)?) -> Void)

Instantiates and returns a source query.

## Relationships

### Inherits From

- HKQuery

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Sources and devices

struct HKSourceQueryDescriptor

A query interface that uses Swift concurrency to read the apps and devices that produced the matching samples.

class HKSourceRevision

An object indicating the source of a HealthKit sample.

class HKSource

An object indicating the app or device that created a HealthKit sample

class HKDevice

A device that generates data for HealthKit.

