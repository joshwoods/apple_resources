

- XCUIAutomation
- XCUIElement
-  typeText(\_:) 

Instance Method

# typeText(\_:)

Types a string into the element.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSXcode 16.3+

``` source
@MainActor
func typeText(_ text: String)
```

## Discussion

The element or a descendant must have keyboard focus; otherwise the system raises an error. This API discards any modifiers set in the current context by perform(withKeyModifiers:block:) so that it strictly interprets the provided text. To input keys with modifier flags, use typeKey(_:modifierFlags:).

