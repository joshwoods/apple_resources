

- SensorKit
-  SRFetchRequest 

Class

# SRFetchRequest

An object that defines the criteria for a sample query.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
class SRFetchRequest
```

## Overview

An app configures an instance of this class to select the device from which to query sensor data. The time range (from, to) specifies when the framework records the data. A fetch query can retrieve only sensor data that the app records by first calling startRecording().

To execute a fetch request, an app passes the instance of this class to its sensor reader’s fetch(_:) function.

The framework notifies the sensor reader’s delegate upon fetch-request completion with sensorReader(_:didCompleteFetch:). If the fetch fails, the framework calls the delegate’s sensorReader(_:fetching:failedWithError:).

SensorKit places a 24-hour holding period on newly recorded data before an app can access it. This gives the user an opportunity to delete any data they don’t want to share with the app. A fetch request doesn’t return any results if its time range overlaps this holding period.

## Topics

### Selecting the Device

var device: SRDevice

The device to query for sample data.

class SRDevice

A representation of a device that provides sample data.

### Defining the Time Range

var from: SRAbsoluteTime

Fetches sample information that occurs after this time.

var to: SRAbsoluteTime

Fetches sample information that occurs before this time.

struct SRAbsoluteTime

A value that describes when the system records the data.

static func current() -> SRAbsoluteTime

Provides the current absolute time.

func toCFAbsoluteTime() -> CFAbsoluteTime

Converts an absolute time to a core-foundation absolute time.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Querying data

class SRFetchResult

Recorded data that a sensor reader fetches.

