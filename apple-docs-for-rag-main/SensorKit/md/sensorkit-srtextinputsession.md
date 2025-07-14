

- SensorKit
-  SRTextInputSession 

Class

# SRTextInputSession

The characters a user types for a particular keyboard.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
class SRTextInputSession
```

## Overview

The framework instantiates a new instance of this class every time the keyboard displays after dismissal.

## Topics

### Identifying the Session

var sessionIdentifier: String

A unique identifier for the keyboard session.

### Timing Text Input

var duration: TimeInterval

The length of time, in seconds, that the session spans.

### Inspecting Text Source

var sessionType: SRTextInputSession.SessionType

enum SessionType

Methods to input text during a session.

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

### Inspecting Text Input

var textInputSessions: [SRTextInputSession]

The text input session types that occur during application usage.

