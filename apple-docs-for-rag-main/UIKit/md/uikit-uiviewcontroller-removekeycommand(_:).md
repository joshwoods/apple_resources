

- UIKit
- UIViewController
-  removeKeyCommand(\_:) 

Instance Method

# removeKeyCommand(\_:)

Removes the key command from the view controller.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
func removeKeyCommand(_ keyCommand: UIKeyCommand)
```

## Parameters 

`keyCommand`  

The key command to remove.

## Discussion

This method lets you easily remove key commands without overriding the keyCommands property.

## See Also

### Related Documentation

var keyCommands: [UIKeyCommand]?

The key commands that trigger actions on this responder.

### Accessing the available key commands

var performsActionsWhilePresentingModally: Bool

A Boolean value indicating whether the view controller performs menu-related actions.

func addKeyCommand(UIKeyCommand)

Associates the specified keyboard shortcut with the view controller.

