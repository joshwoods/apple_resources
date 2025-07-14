

- CallKit
- CXPlayDTMFCallAction
-  CXPlayDTMFCallAction.ActionType 

Enumeration

# CXPlayDTMFCallAction.ActionType

The types of events that generate dial tones.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
enum ActionType
```

## Topics

### Constants

case singleTone

Indicates that the user tapped a digit on the in-call keypad.

case softPause

Indicates that the user included digits after a soft pause in their dial string. A soft pause is indicated by a comma (`,`) and waits a few seconds before dialing the additional digits.

case hardPause

Indicates that the user included digits after a hard pause in their dial string. A hard pause is indicated by a semicolon (`;`) and waits for further user interaction before dialing the additional digits.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

