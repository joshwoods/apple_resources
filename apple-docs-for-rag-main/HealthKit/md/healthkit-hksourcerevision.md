

- HealthKit
-  HKSourceRevision 

Class

# HKSourceRevision

An object indicating the source of a HealthKit sample.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
class HKSourceRevision
```

## Mentioned in 

About the HealthKit framework

## Overview

The HKSourceRevision class acts as a wrapper for the HKSource class, adding information about the source’s version, operating system, and product type.

Source revision objects are immutable: you set the source revision’s properties when you create the object, and they cannot change.

When an HKObject instance is created, its sourceRevision property is set to `nil`. When the object is saved to the HealthKit store, HealthKit assigns a new source revision to the object’s sourceRevision property. The source revision can be accessed only on objects retrieved from the HealthKit store.

### Subclassing Source Revisions

Like many HealthKit classes, the HKSourceRevision class is not extensible and should not be subclassed.

## Topics

### Creating Source Revision Objects

init(source: HKSource, version: String?)

Initializes a new source revision object with the provided source and version information.

init(source: HKSource, version: String?, productType: String?, operatingSystemVersion: OperatingSystemVersion)

Initializes a new source revision object with the provided source, version, product type, and operating system.

### Accessing Source and Version Information

var source: HKSource

The source for a sample.

var version: String?

A string that identifies a particular version of the source.

var operatingSystemVersion: OperatingSystemVersion

A string that identifies the operating system used to save a sample.

var productType: String?

A string that identifies the device used to save a sample.

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

class HKSource

An object indicating the app or device that created a HealthKit sample

class HKDevice

A device that generates data for HealthKit.

class HKSourceQuery

A query that returns a list of sources, such as apps and devices, that have saved matching queries to the HealthKit store.

