

- SensorKit
- SRElectrocardiogramSession
-  state 

Instance Property

# state

The state of the session used to record the sample.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+

``` source
var state: SRElectrocardiogramSession.State { get }
```

## See Also

### Getting session information

var identifier: String

A unique identifier for the ECG session.

var sessionGuidance: SRElectrocardiogramSession.SessionGuidance

The type of session used to record the sample.

enum SessionGuidance

The type of session guidance used to record a ECG sample.

enum State

The state of a session used to record a ECG sample.

