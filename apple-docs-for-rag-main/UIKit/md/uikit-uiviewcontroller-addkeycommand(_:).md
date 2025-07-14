

- UIKit
- UIViewController
-  addKeyCommand(\_:) 

Instance Method

# addKeyCommand(\_:)

Associates the specified keyboard shortcut with the view controller.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
func addKeyCommand(_ keyCommand: UIKeyCommand)
```

## Parameters 

`keyCommand`  

The key command to add.

## Discussion

This method lets you easily add key commands to the view controller without overriding the keyCommands property. The key commands you add to a view controller are applied to the active responder chain. When the user performs a key command, UIKit searches the responder chain (starting with the first responder) for an object capable of handling the specified action.

## See Also

### Related Documentation

var keyCommands: [UIKeyCommand]?

The key commands that trigger actions on this responder.

### Accessing the available key commands

var performsActionsWhilePresentingModally: Bool

A Boolean value indicating whether the view controller performs menu-related actions.

func removeKeyCommand(UIKeyCommand)

Removes the key command from the view controller.

