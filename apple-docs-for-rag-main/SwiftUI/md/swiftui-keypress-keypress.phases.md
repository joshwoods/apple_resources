

- SwiftUI
- KeyPress
-  KeyPress.Phases 

Structure

# KeyPress.Phases

Options for matching different phases of a key-press event.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
struct Phases
```

## Topics

### Getting the phases

static let down: KeyPress.Phases

The user pressed down on a key.

static let up: KeyPress.Phases

The user released a key.

static let `repeat`: KeyPress.Phases

The user held a key down to issue a sequence of repeating events.

static let all: KeyPress.Phases

A value that matches all key press phases.

## Relationships

### Conforms To

- CustomDebugStringConvertible
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Getting the phase of the keypress

let phase: KeyPress.Phases

The phase of the key-press event (`.down`, `.repeat`, or `.up`).

