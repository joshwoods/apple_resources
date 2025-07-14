

- InputMethodKit
- IMKInputController
-  doCommand(by:command:) 

Instance Method

# doCommand(by:command:)

Passes commands that are not generated as part of the text input process.

macOS 10.5+

``` source
func doCommand(
    by aSelector: Selector!,
    command infoDictionary: [AnyHashable : Any]!
)
```

## Parameters 

`aSelector`  

A selector that represents a command from the text input menu.

`infoDictionary`  

A dictionary that contains two key-value pairs:

- kIMKCommandMenuItemName, whose value is an `NSMenuItem` object. That is, the item selected by the user.

- kIMKCommandClientName, whose value is the current client—`id`.

## Discussion

The default implementation checks if the input controller object (that is, self) responds to the selector. If so, it sends the message perform(_:with:) to the input controller class. The object parameter in that case is the `infoDictionary` parameter.

This method is called when a user selects a command from the text input menu. To support this, an input method must provide actions for each menu item that is placed in the menu. For example, `(void)menuAction:(id)sender`. Note that the sender in this instance is the info dictionary.

## See Also

### Working with Custom Commands

func menu() -> NSMenu!

Returns a menu of commands that are specific to an input method.

