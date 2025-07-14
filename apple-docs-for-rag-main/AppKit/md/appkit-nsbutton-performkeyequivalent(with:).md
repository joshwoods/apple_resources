

- AppKit
- NSButton
-  performKeyEquivalent(with:) 

Instance Method

# performKeyEquivalent(with:)

Checks the button’s key equivalent against the specified event and, if they match, simulates the button being clicked.

macOS

``` source
@MainActor
func performKeyEquivalent(with key: NSEvent) -> Bool
```

## Parameters 

`key`  

The event containing the key equivalent.

## Return Value

true if the key equivalent in `anEvent` matches the button’s key equivalent; false if it does not. This method also returns false if the button is blocked by a modal panel or the button is disabled.

## Discussion

If the character in `anEvent` matches the button’s key equivalent, and the modifier flags in `anEvent` match the key-equivalent modifier mask, performKeyEquivalent(with:) simulates the user clicking the button and returning true. Otherwise, performKeyEquivalent(with:) does nothing and returns false.

## See Also

### Related Documentation

var keyEquivalent: String

The key-equivalent character of the button.

var keyEquivalentModifierMask: NSEvent.ModifierFlags

The mask specifying the modifier keys for the button’s key equivalent.

