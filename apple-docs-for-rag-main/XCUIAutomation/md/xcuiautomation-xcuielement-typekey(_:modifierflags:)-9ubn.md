

- XCUIAutomation
- XCUIElement
-  typeKey(\_:modifierFlags:) 

Instance Method

# typeKey(\_:modifierFlags:)

Types a single key that a string represents with the flags you specify.

iOSiPadOSMac CatalystmacOSXcode 16.3+

``` source
@MainActor
func typeKey(
    _ key: String,
    modifierFlags flags: XCUIElement.KeyModifierFlags
)
```

## Parameters 

`key`  

A string representation of the key to type, or a constant from XCUIKeyboardKey for a key that doesn’t have a single-key string equivalent.

`flags`  

A set of modifier flags (XCUIElement.KeyModifierFlags) to use when typing the key.

## Discussion

Although `key` is a string, it must represent a single key on a physical keyboard. Strings that resolve to multiple keys raise an error at runtime.

In addition to literal string key representations like `"a"`, `"6"`, and `"["`, keys such as arrow keys, Command, Control, Option, and function keys can be typed using the constants in XCUIKeyboardKey.

## See Also

### Combining keystrokes

func typeKey(XCUIKeyboardKey, modifierFlags: XCUIElement.KeyModifierFlags)

Types a single key from the XCUIKeyboardKey enumeration with the specified modifier flags.

struct XCUIKeyboardKey

Constants to represent keys that have no typewritten equivalent.

class func perform(withKeyModifiers: XCUIElement.KeyModifierFlags, block: () -> Void)

Executes a block of code while holding a combination keystroke.

struct KeyModifierFlags

Flags for simulating combination keystrokes with keys, such as Control, Option, Shift, and Command.

