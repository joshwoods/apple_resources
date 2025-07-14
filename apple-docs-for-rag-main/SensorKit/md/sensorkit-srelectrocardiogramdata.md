

- SensorKit
-  SRElectrocardiogramData 

Class

# SRElectrocardiogramData

A representation of the ECG data that the sensor records.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+

``` source
class SRElectrocardiogramData
```

## Topics

### Getting electrocardiogram details

var flags: SRElectrocardiogramData.Flags

struct Flags

Sensor context or events that occur during a sample ECG data reading.

var value: Measurement&lt;UnitElectricPotentialDifference>

The electrocardiogram data in microvolts.

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

### Accessing ECG data

var date: Date

The start date of the ECG sensor data recording, not the start of the session.

var frequency: Measurement&lt;UnitFrequency>

The frequency in hertz that the ECG sensor records the data.

var lead: SRElectrocardiogramSample.Lead

The lead used to record the ECG data.

enum Lead

The location of the lead that a person uses to record the ECG data.

var session: SRElectrocardiogramSession

The session where this sample occurs.

class SRElectrocardiogramSession

An object that represents ECG data that a device records during a period of time.

var data: [SRElectrocardiogramData]

The data that the sensor records.

