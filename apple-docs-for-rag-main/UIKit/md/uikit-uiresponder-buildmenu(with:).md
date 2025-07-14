

- UIKit
- UIResponder
-  buildMenu(with:) 

Instance Method

# buildMenu(with:)

Asks the receiving responder to add and remove items from a menu system.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
func buildMenu(with builder: any UIMenuBuilder)
```

## Parameters 

`builder`  

An object that you use to modify a menu system for your app.

## Discussion

Override this method in your app delegate or view controller to receive a UIMenuBuilder object. Use the builder to add and remove UIMenuElement objects such as UIMenu, UIAction, and UICommand from your app’s menu bar or context menus.

Note

The menu bar is available in Mac apps built with Mac Catalyst.

Where you override this method determines the menu system that the builder updates. To add and remove items from the menu bar using the main menu system, override buildMenu(with:) in your app delegate. To build a context menu using the context system, override this method in your view controller.

## See Also

### Building and validating commands

func validate(UICommand)

Asks the receiving responder to validate the command.

func canPerformAction(Selector, withSender: Any?) -> Bool

Requests the receiving responder to enable or disable the specified command in the user interface.

func target(forAction: Selector, withSender: Any?) -> Any?

Returns the target object that responds to an action.

