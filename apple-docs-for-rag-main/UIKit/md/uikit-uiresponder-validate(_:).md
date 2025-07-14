

- UIKit
- UIResponder
-  validate(\_:) 

Instance Method

# validate(\_:)

Asks the receiving responder to validate the command.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
func validate(_ command: UICommand)
```

## Parameters 

`command`  

A mutable command object.

## Discussion

Override this method in your view controller to make changes to a command before the command system renders it as a menu item.

## See Also

### Building and validating commands

func buildMenu(with: any UIMenuBuilder)

Asks the receiving responder to add and remove items from a menu system.

func canPerformAction(Selector, withSender: Any?) -> Bool

Requests the receiving responder to enable or disable the specified command in the user interface.

func target(forAction: Selector, withSender: Any?) -> Any?

Returns the target object that responds to an action.

