

- SensorKit
-  SRElectrocardiogramSession 

Class

# SRElectrocardiogramSession

An object that represents ECG data that a device records during a period of time.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+

``` source
class SRElectrocardiogramSession
```

## Topics

### Getting session information

var identifier: String

A unique identifier for the ECG session.

var sessionGuidance: SRElectrocardiogramSession.SessionGuidance

The type of session used to record the sample.

enum SessionGuidance

The type of session guidance used to record a ECG sample.

var state: SRElectrocardiogramSession.State

The state of the session used to record the sample.

enum State

The state of a session used to record a ECG sample.

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

var data: [SRElectrocardiogramData]

The data that the sensor records.

class SRElectrocardiogramData

A representation of the ECG data that the sensor records.

