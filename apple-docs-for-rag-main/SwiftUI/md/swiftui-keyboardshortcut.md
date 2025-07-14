

- SwiftUI
-  KeyboardShortcut 

Structure

# KeyboardShortcut

Keyboard shortcuts describe combinations of keys on a keyboard that the user can press in order to activate a button or toggle.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
struct KeyboardShortcut
```

## Topics

### Getting standard shortcuts

static let cancelAction: KeyboardShortcut

The standard keyboard shortcut for cancelling the in-progress action or dismissing a prompt, consisting of the Escape (⎋) key and no modifiers.

static let defaultAction: KeyboardShortcut

The standard keyboard shortcut for the default button, consisting of the Return (↩) key and no modifiers.

### Creating a shortcut

init(KeyEquivalent, modifiers: EventModifiers)

Creates a new keyboard shortcut with the given key equivalent and set of modifier keys.

var key: KeyEquivalent

The key equivalent that the user presses in conjunction with any specified modifier keys to activate the shortcut.

var modifiers: EventModifiers

The modifier keys that the user presses in conjunction with a key equivalent to activate the shortcut.

### Creating a localized shortcut

init(KeyEquivalent, modifiers: EventModifiers, localization: KeyboardShortcut.Localization)

Creates a new keyboard shortcut with the given key equivalent and set of modifier keys.

var localization: KeyboardShortcut.Localization

The localization strategy to apply to this shortcut.

struct Localization

Options for how a keyboard shortcut participates in automatic localization.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

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

struct KeyEquivalent

Key equivalents consist of a letter, punctuation, or function key that can be combined with an optional set of modifier keys to specify a keyboard shortcut.

struct EventModifiers

A set of key modifiers that you can add to a gesture.

