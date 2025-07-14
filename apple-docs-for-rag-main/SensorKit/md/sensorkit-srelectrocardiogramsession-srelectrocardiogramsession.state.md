

- SensorKit
- SRElectrocardiogramSession
-  SRElectrocardiogramSession.State 

Enumeration

# SRElectrocardiogramSession.State

The state of a session used to record a ECG sample.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+

``` source
enum State
```

## Topics

### States

case begin

The session begins.

case active

The session is ongoing.

case end

The session ends.

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

enum SessionGuidance

The type of session guidance used to record a ECG sample.

var state: SRElectrocardiogramSession.State

The state of the session used to record the sample.

