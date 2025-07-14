

- AppKit
- NSAlert
-  buttons 

Instance Property

# buttons

The array of response buttons for the alert.

macOS

``` source
@MainActor
var buttons: [NSButton] { get }
```

## Discussion

The button displayed rightmost in the alert (for a left-to-right language) corresponds to the button at index `0` in this property’s array, and is considered the default button. A user can invoke this button by pressing the Return key.

Any button with a title of “Cancel” has a key equivalent of Escape, and any button with the title “Don’t Save” has a key equivalent of Command-D (but only if it is not the first button). You can also assign different key equivalents for the buttons using the keyEquivalent method of the `NSButton` class.

## See Also

### Accessing Alert Response Buttons

func addButton(withTitle: String) -> NSButton

Adds a button with a given title to the alert.

