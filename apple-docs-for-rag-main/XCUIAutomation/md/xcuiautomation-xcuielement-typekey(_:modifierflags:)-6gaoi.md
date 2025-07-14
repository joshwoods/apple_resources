

- XCUIAutomation
- XCUIElement
-  typeKey(\_:modifierFlags:) 

Instance Method

# typeKey(\_:modifierFlags:)

Types a single key from the XCUIKeyboardKey enumeration with the specified modifier flags.

iOSiPadOSMac CatalystmacOSvisionOSSwift 4.0+Xcode 16.3+

``` source
@MainActor @nonobjc @preconcurrency
func typeKey(
    _ key: XCUIKeyboardKey,
    modifierFlags: XCUIElement.KeyModifierFlags
)
```

## See Also

### Combining keystrokes

func typeKey(String, modifierFlags: XCUIElement.KeyModifierFlags)

Types a single key that a string represents with the flags you specify.

struct XCUIKeyboardKey

Constants to represent keys that have no typewritten equivalent.

class func perform(withKeyModifiers: XCUIElement.KeyModifierFlags, block: () -> Void)

Executes a block of code while holding a combination keystroke.

struct KeyModifierFlags

Flags for simulating combination keystrokes with keys, such as Control, Option, Shift, and Command.

