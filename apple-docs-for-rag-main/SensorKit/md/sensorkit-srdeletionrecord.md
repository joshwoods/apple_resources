

- SensorKit
-  SRDeletionRecord 

Class

# SRDeletionRecord

An object that describes the reason the framework deletes samples.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
class SRDeletionRecord
```

## Overview

When there are gaps in a recorded sensor’s data, deletion records account for the occasions when the framework deliberately removes the records. A deletion record specifies the time range when records are unavailable (see startTime and endTime), and the reason for removal.

To access deletion records for a particular sensor, create a new reader by applying the `sr_sensorForDeletionRecordsFromSensor()` extension of NSString to the source sensor.

```
let deletionRecordsReader = SRSensorReader(sensor: ambientLightSensor.rawValue.sr_sensorForDeletionRecordsFromSensor())
deletionRecordsReader.delegate = myAmbientLightDeletionRecordsDelegate
```

## Topics

### Accessing the Deletion Reason

var reason: SRDeletionReason

The reason the framework deletes samples.

enum SRDeletionReason

Reasons that the framework deletes samples.

### Accessing the Deletion Time

var startTime: SRAbsoluteTime

The time the framework begins deleting samples.

var endTime: SRAbsoluteTime

The time the framework finishes deleting samples.

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
- NSObjectProtocol
- NSSecureCoding

