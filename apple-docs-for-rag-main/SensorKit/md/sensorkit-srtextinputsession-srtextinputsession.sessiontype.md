

- SensorKit
- SRTextInputSession
-  SRTextInputSession.SessionType 

Enumeration

# SRTextInputSession.SessionType

Methods to input text during a session.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
enum SessionType
```

## Overview

This class defines available options for the sessionType property.

## Topics

### Sources

case dictation

Indicates that the session contains spoken text.

case keyboard

Indicates that the session contains text from keyboard input.

case pencil

Indicates that the session contains text drawn with Apple Pencil.

case thirdPartyKeyboard

Indicates that the session contains text from a third-party keyboard.

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

### Inspecting Text Source

var sessionType: SRTextInputSession.SessionType

