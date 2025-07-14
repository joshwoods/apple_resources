

- XCUIAutomation
- XCUIElement
-  XCUIElement.KeyModifierFlags 

Structure

# XCUIElement.KeyModifierFlags

Flags for simulating combination keystrokes with keys, such as Control, Option, Shift, and Command.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSXcode 16.3+

``` source
struct KeyModifierFlags
```

## Overview

Use these flags with the typeKey(_:modifierFlags:) and perform(withKeyModifiers:block:) methods to simulate combination keystrokes while an action occurs.

## Topics

### Flags for combination keys

static var command: XCUIElement.KeyModifierFlags

The Command key in a combination keystroke.

static var control: XCUIElement.KeyModifierFlags

The Control key in a combination keystroke.

static var option: XCUIElement.KeyModifierFlags

The Option key in a combination keystroke.

static var shift: XCUIElement.KeyModifierFlags

The Shift key in a combination keystroke.

static var capsLock: XCUIElement.KeyModifierFlags

The Caps Lock key in a combination keystroke.

static var function: XCUIElement.KeyModifierFlags

The Function key in a combination keystroke.

### Initializers

init(rawValue: UInt)

Creates a flag that represents a key in a combination keystroke with the specified raw value.

### Legacy flags for combination keys

static var alphaShift: XCUIElement.KeyModifierFlags

The Caps Lock key in a combination keystroke.

static var alternate: XCUIElement.KeyModifierFlags

The Option key in a combination keystroke.

### Default Implementations

Equatable Implementations

OptionSet Implementations

SetAlgebra Implementations

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Combining keystrokes

func typeKey(XCUIKeyboardKey, modifierFlags: XCUIElement.KeyModifierFlags)

Types a single key from the XCUIKeyboardKey enumeration with the specified modifier flags.

func typeKey(String, modifierFlags: XCUIElement.KeyModifierFlags)

Types a single key that a string represents with the flags you specify.

struct XCUIKeyboardKey

Constants to represent keys that have no typewritten equivalent.

class func perform(withKeyModifiers: XCUIElement.KeyModifierFlags, block: () -> Void)

Executes a block of code while holding a combination keystroke.

