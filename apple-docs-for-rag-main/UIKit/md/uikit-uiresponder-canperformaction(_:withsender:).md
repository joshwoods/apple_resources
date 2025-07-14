

- UIKit
- UIResponder
-  canPerformAction(\_:withSender:) 

Instance Method

# canPerformAction(\_:withSender:)

Requests the receiving responder to enable or disable the specified command in the user interface.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func canPerformAction(
    _ action: Selector,
    withSender sender: Any?
) -> Bool
```

## Parameters 

`action`  

A selector that identifies a method associated with a command. For the editing menu, this is one of the editing methods declared by the UIResponderStandardEditActions informal protocol (for example, `copy:`).

`sender`  

The object calling this method. For the editing menu commands, this is the shared UIApplication object. Depending on the context, you can query the sender for information to help you determine whether a command should be enabled.

## Return Value

true if the command identified by `action` should be enabled or false if it should be disabled. Returning true means that your class can handle the command in the current context.

## Discussion

This default implementation of this method returns true if the responder class implements the requested action and calls the next responder if it doesn’t. Subclasses may override this method to enable menu commands based on the current state; for example, you would enable the Copy command if there’s a selection or disable the Paste command if the pasteboard didn’t contain data with the correct pasteboard representation type. If no responder in the responder chain returns true, the menu command is disabled. Note that if your class returns false for a command, another responder further up the responder chain may still return true, enabling the command.

This method might be called more than once for the same action but with a different sender each time. You should be prepared for any kind of sender including `nil`.

For information on the editing menu, see the description of the UIMenuController class.

## See Also

### Building and validating commands

func buildMenu(with: any UIMenuBuilder)

Asks the receiving responder to add and remove items from a menu system.

func validate(UICommand)

Asks the receiving responder to validate the command.

func target(forAction: Selector, withSender: Any?) -> Any?

Returns the target object that responds to an action.

