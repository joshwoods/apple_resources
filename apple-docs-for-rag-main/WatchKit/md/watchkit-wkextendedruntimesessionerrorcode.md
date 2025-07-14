

- WatchKit
-  WKExtendedRuntimeSessionErrorCode 

Enumeration

# WKExtendedRuntimeSessionErrorCode

The error codes reported by extended runtime sessions.

watchOS 6.0+

``` source
enum WKExtendedRuntimeSessionErrorCode
```

## Overview

The session passes these errors to the sesson delegate’s extendedRuntimeSession(_:didInvalidateWith:error:) method.

## Topics

### Error Codes

case unknown

An unknown error occurred.

case scheduledTooFarInAdvance

The app attempted to schedule a session too far in the future.

case mustBeActiveToStartOrSchedule

The watchOS app attempted to start or schedule a session while not in an active state.

case notYetStarted

The app invalidated the session before it started.

case exceededResourceLimits

The session exceeded its resource limits.

case barDisabled

The user has disabled background app refresh.

case notApprovedToStartSession

The app attempted to start a session, but doesn’t have a valid session type.

case notApprovedToSchedule

The app attempted to schedule a session, but the session type does not support scheduling.

### Enumeration Cases

case mustBeActiveToPrompt

case unsupportedSessionType

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

### Handling Errors

let WKExtendedRuntimeSessionErrorDomain: String

The domain for errors reported by extended runtime sessions.

