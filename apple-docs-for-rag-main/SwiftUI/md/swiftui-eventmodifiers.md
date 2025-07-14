

- SwiftUI
-  EventModifiers 

Structure

# EventModifiers

A set of key modifiers that you can add to a gesture.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@frozen
struct EventModifiers
```

## Topics

### Getting modifier keys

static let all: EventModifiers

All possible modifier keys.

static let capsLock: EventModifiers

The Caps Lock key.

static let command: EventModifiers

The Command key.

static let control: EventModifiers

The Control key.

static let numericPad: EventModifiers

Any key on the numeric keypad.

static let option: EventModifiers

The Option key.

static let shift: EventModifiers

The Shift key.

### Creating a set of options

init(rawValue: Int)

Creates a new set from a raw value.

let rawValue: Int

The raw value.

### Deprecated modifiers

static let function: EventModifiers

The Function key.

Deprecated

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Creating keyboard shortcuts

func keyboardShortcut(_:)

Assigns a keyboard shortcut to the modified control.

func keyboardShortcut(KeyEquivalent, modifiers: EventModifiers) -> some View

Defines a keyboard shortcut and assigns it to the modified control.

func keyboardShortcut(KeyEquivalent, modifiers: EventModifiers, localization: KeyboardShortcut.Localization) -> some View

Defines a keyboard shortcut and assigns it to the modified control.

var keyboardShortcut: KeyboardShortcut?

The keyboard shortcut that buttons in this environment will be triggered with.

struct KeyboardShortcut

Keyboard shortcuts describe combinations of keys on a keyboard that the user can press in order to activate a button or toggle.

struct KeyEquivalent

Key equivalents consist of a letter, punctuation, or function key that can be combined with an optional set of modifier keys to specify a keyboard shortcut.

