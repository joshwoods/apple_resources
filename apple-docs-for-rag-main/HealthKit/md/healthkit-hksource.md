

- HealthKit
-  HKSource 

Class

# HKSource

An object indicating the app or device that created a HealthKit sample

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
class HKSource
```

## Overview

Sources include apps and devices that save data to the HealthKit store. Currently, HealthKit supports only the direct import of data from Bluetooth LE heart rate monitors. All other devices need a companion app to collect and save the data to HealthKit.

## Topics

### Getting the Current Source

class func `default`() -> HKSource

Returns a source object for the current app.

### Getting Property Data

var bundleIdentifier: String

The source’s bundle identifier.

var name: String

The source’s name.

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

### Sources and devices

struct HKSourceQueryDescriptor

A query interface that uses Swift concurrency to read the apps and devices that produced the matching samples.

class HKSourceRevision

An object indicating the source of a HealthKit sample.

class HKDevice

A device that generates data for HealthKit.

class HKSourceQuery

A query that returns a list of sources, such as apps and devices, that have saved matching queries to the HealthKit store.

