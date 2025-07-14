

- XCUIAutomation
- XCUIElement
-  perform(withKeyModifiers:block:) 

Type Method

# perform(withKeyModifiers:block:)

Executes a block of code while holding a combination keystroke.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOSXcode 16.3+

``` source
@MainActor
class func perform(
    withKeyModifiers flags: XCUIElement.KeyModifierFlags,
    block: () -> Void
)
```

## Parameters 

`flags`  

A set of modifier flags (XCUIElement.KeyModifierFlags) to use while executing the block.

`block`  

The block to execute.

## Discussion

This method sets and holds the keyboard modifiers you provide while you call methods to click on, drag from, or type into elements in the block.

## See Also

### Combining keystrokes

func typeKey(XCUIKeyboardKey, modifierFlags: XCUIElement.KeyModifierFlags)

Types a single key from the XCUIKeyboardKey enumeration with the specified modifier flags.

func typeKey(String, modifierFlags: XCUIElement.KeyModifierFlags)

Types a single key that a string represents with the flags you specify.

struct XCUIKeyboardKey

Constants to represent keys that have no typewritten equivalent.

struct KeyModifierFlags

Flags for simulating combination keystrokes with keys, such as Control, Option, Shift, and Command.

