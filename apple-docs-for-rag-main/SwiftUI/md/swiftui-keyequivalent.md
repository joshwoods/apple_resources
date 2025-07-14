

- SwiftUI
-  KeyEquivalent 

Structure

# KeyEquivalent

Key equivalents consist of a letter, punctuation, or function key that can be combined with an optional set of modifier keys to specify a keyboard shortcut.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 17.0+visionOS 1.0+

``` source
struct KeyEquivalent
```

## Overview

Key equivalents are used to establish keyboard shortcuts to app functionality. Any key can be used as a key equivalent as long as pressing it produces a single character value. Key equivalents are typically initialized using a single-character string literal, with constants for unprintable or hard-to-type values.

The modifier keys necessary to type a key equivalent are factored in to the resulting keyboard shortcut. That is, a key equivalent whose raw value is the capitalized string “A” corresponds with the keyboard shortcut Command-Shift-A. The exact mapping may depend on the keyboard layout—for example, a key equivalent with the character value “}” produces a shortcut equivalent to Command-Shift-\] on ANSI keyboards, but would produce a different shortcut for keyboard layouts where punctuation characters are in different locations.

## Topics

### Getting arrow keys

static let upArrow: KeyEquivalent

Up Arrow (U+F700)

static let downArrow: KeyEquivalent

Down Arrow (U+F701)

static let leftArrow: KeyEquivalent

Left Arrow (U+F702)

static let rightArrow: KeyEquivalent

Right Arrow (U+F703)

### Getting other special keys

static let clear: KeyEquivalent

Clear (U+F739)

static let delete: KeyEquivalent

Delete (U+0008)

static let deleteForward: KeyEquivalent

Delete Forward (U+F728)

static let end: KeyEquivalent

End (U+F72B)

static let escape: KeyEquivalent

Escape (U+001B)

static let home: KeyEquivalent

Home (U+F729)

static let pageDown: KeyEquivalent

Page Down (U+F72D)

static let pageUp: KeyEquivalent

Page Up (U+F72C)

static let `return`: KeyEquivalent

Return (U+000D)

static let space: KeyEquivalent

Space (U+0020)

static let tab: KeyEquivalent

Tab (U+0009)

### Creating a key equivalent

init(Character)

Creates a new key equivalent from the given character value.

var character: Character

The character value that the key equivalent represents.

## Relationships

### Conforms To

- Copyable
- Equatable
- ExpressibleByExtendedGraphemeClusterLiteral
- ExpressibleByUnicodeScalarLiteral
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

struct KeyboardShortcut

Keyboard shortcuts describe combinations of keys on a keyboard that the user can press in order to activate a button or toggle.

struct EventModifiers

A set of key modifiers that you can add to a gesture.

