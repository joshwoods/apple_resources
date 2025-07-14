

- SensorKit
- SRElectrocardiogramSession
-  SRElectrocardiogramSession.SessionGuidance 

Enumeration

# SRElectrocardiogramSession.SessionGuidance

The type of session guidance used to record a ECG sample.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+

``` source
enum SessionGuidance
```

## Topics

### Types

case guided

The system coaches the user to guide the ECG readings.

case unguided

The system doesn’t coach the user to guide the ECG readings.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting session information

var identifier: String

A unique identifier for the ECG session.

var sessionGuidance: SRElectrocardiogramSession.SessionGuidance

The type of session used to record the sample.

var state: SRElectrocardiogramSession.State

The state of the session used to record the sample.

enum State

The state of a session used to record a ECG sample.

