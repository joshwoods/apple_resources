

- XCUIAutomation
-  XCUIKeyboardKey 

Structure

# XCUIKeyboardKey

Constants to represent keys that have no typewritten equivalent.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSXcode 16.3+

``` source
struct XCUIKeyboardKey
```

## Discussion

These constants represent the set of modifier, navigation, function, and other keys on most keyboards.

## Topics

### Modifier keys

static let command: XCUIKeyboardKey

A constant that represents the Command key.

static let control: XCUIKeyboardKey

A constant that represents the Control key.

static let option: XCUIKeyboardKey

A constant that represents the Option key.

static let shift: XCUIKeyboardKey

A constant that represents the Shift key.

static let rightCommand: XCUIKeyboardKey

A constant that represents the right Command key.

static let rightControl: XCUIKeyboardKey

A constant that represents the right Control key.

static let rightOption: XCUIKeyboardKey

A constant that represents the right Option key.

static let rightShift: XCUIKeyboardKey

A constant that represents the right Shift key.

### Navigation keys

static let upArrow: XCUIKeyboardKey

A constant that represents the Up Arrow key.

static let downArrow: XCUIKeyboardKey

A constant that represents the Down Arrow key.

static let leftArrow: XCUIKeyboardKey

A constant that represents the Left Arrow key.

static let rightArrow: XCUIKeyboardKey

A constant that represents the Right Arrow key.

static let home: XCUIKeyboardKey

A constant that represents the Home key.

static let end: XCUIKeyboardKey

A constant that represents the End key.

static let pageUp: XCUIKeyboardKey

A constant that represents the Page Up key.

static let pageDown: XCUIKeyboardKey

A constant that represents the Page Down key.

static let help: XCUIKeyboardKey

A constant that represents the Help key.

### Function keys

static let secondaryFn: XCUIKeyboardKey

A constant that represents the Function key.

static let F1: XCUIKeyboardKey

A constant that represents the F1 key.

static let F2: XCUIKeyboardKey

A constant that represents the F2 key.

static let F3: XCUIKeyboardKey

A constant that represents the F3 key.

static let F4: XCUIKeyboardKey

A constant that represents the F4 key.

static let F5: XCUIKeyboardKey

A constant that represents the F5 key.

static let F6: XCUIKeyboardKey

A constant that represents the F6 key.

static let F7: XCUIKeyboardKey

A constant that represents the F7 key.

static let F8: XCUIKeyboardKey

A constant that represents the F8 key.

static let F9: XCUIKeyboardKey

A constant that represents the F9 key.

static let F10: XCUIKeyboardKey

A constant that represents the F10 key.

static let F11: XCUIKeyboardKey

A constant that represents the F11 key.

static let F12: XCUIKeyboardKey

A constant that represents the F12 key.

static let F13: XCUIKeyboardKey

A constant that represents the F13 key.

static let F14: XCUIKeyboardKey

A constant that represents the F14 key.

static let F15: XCUIKeyboardKey

A constant that represents the F15 key.

static let F16: XCUIKeyboardKey

A constant that represents the F16 key.

static let F17: XCUIKeyboardKey

A constant that represents the F17 key.

static let F18: XCUIKeyboardKey

A constant that represents the F18 key.

static let F19: XCUIKeyboardKey

A constant that represents the F19 key.

### Text-editing keys

static let capsLock: XCUIKeyboardKey

A constant that represents the Caps Lock key.

static let delete: XCUIKeyboardKey

A constant that represents the Delete key.

static let forwardDelete: XCUIKeyboardKey

A constant that represents the Forward Delete key.

static let space: XCUIKeyboardKey

A constant that represents the Space bar.

static let tab: XCUIKeyboardKey

A constant that represents the Tab key.

### Other keys

static let clear: XCUIKeyboardKey

A constant that represents the Clear key.

static let enter: XCUIKeyboardKey

A constant that represents the Enter key.

static let escape: XCUIKeyboardKey

A constant that represents the Escape key.

static let `return`: XCUIKeyboardKey

A constant that represents the Return key.

### Initializers

init(String)

Initializes a constant with a string that represents a keyboard key.

init(rawValue: String)

Initializes a constant with a string that represents a keyboard key.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Combining keystrokes

func typeKey(XCUIKeyboardKey, modifierFlags: XCUIElement.KeyModifierFlags)

Types a single key from the XCUIKeyboardKey enumeration with the specified modifier flags.

func typeKey(String, modifierFlags: XCUIElement.KeyModifierFlags)

Types a single key that a string represents with the flags you specify.

class func perform(withKeyModifiers: XCUIElement.KeyModifierFlags, block: () -> Void)

Executes a block of code while holding a combination keystroke.

struct KeyModifierFlags

Flags for simulating combination keystrokes with keys, such as Control, Option, Shift, and Command.

