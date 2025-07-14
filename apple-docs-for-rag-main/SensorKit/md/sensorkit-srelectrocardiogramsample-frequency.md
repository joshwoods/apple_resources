

- SensorKit
- SRElectrocardiogramSample
-  frequency 

Instance Property

# frequency

The frequency in hertz that the ECG sensor records the data.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+

``` source
var frequency: Measurement { get }
```

## See Also

### Accessing ECG data

var date: Date

The start date of the ECG sensor data recording, not the start of the session.

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

class SRElectrocardiogramData

A representation of the ECG data that the sensor records.

