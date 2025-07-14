

- LiveCommunicationKit
- PlayToneAction
-  PlayToneAction.Tone 

Enumeration

# PlayToneAction.Tone

The types of tones that may be played.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS 1.1+watchOS 10.4+

``` source
enum Tone
```

## Topics

### Enumeration Cases

case hardPause

Indicates that the user included digits after a hard pause in their dial string. A hard pause is indicated by a semicolon (;) and waits for further user interaction before dialing the additional digits.

case single

Indicates that the user tapped a digit on the in-call keypad.

case softPause

Indicates that the user included digits after a soft pause in their dial string. A soft pause is indicated by a comma (,) and waits a few seconds before dialing the additional digits.

### Initializers

init?(rawValue: Int)

Creates a new instance with the specified raw value.

### Instance Properties

var rawValue: Int

The corresponding value of the raw type.

### Type Aliases

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

