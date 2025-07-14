

- AppKit
- NSAlert
-  addButton(withTitle:) 

Instance Method

# addButton(withTitle:)

Adds a button with a given title to the alert.

macOS

``` source
@MainActor
func addButton(withTitle title: String) -> NSButton
```

## Parameters 

`title`  

Title of the button to add to the alert. Must not be `nil`.

## Return Value

Button added to the alert.

## Discussion

Buttons are placed starting near the right side of the alert and going toward the left side (for languages that read left to right). The first three buttons are identified positionally as `NSAlertFirstButtonReturn`, `NSAlertSecondButtonReturn`, `NSAlertThirdButtonReturn` in the return-code parameter evaluated by the modal delegate. Subsequent buttons are identified as `NSAlertThirdButtonReturn` +`n`, where `n` is an integer

By default, the first button has a key equivalent of Return, any button with a title of “Cancel” has a key equivalent of Escape, and any button with the title “Don’t Save” has a key equivalent of Command-D (but only if it’s *not* the first button). You can also assign different key equivalents for the buttons using the keyEquivalent method of the `NSButton` class. In addition, you can use the tag method of the `NSButton` class to set the return value.

## See Also

### Related Documentation

class NSAlert

A modal dialog or sheet attached to a document window.

### Accessing Alert Response Buttons

var buttons: [NSButton]

The array of response buttons for the alert.

