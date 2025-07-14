

- WebKit
- WKWebExtensionContext
-  performCommand(for:) 

Instance Method

# performCommand(for:)

Performs the command associated with the given key command.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+visionOS 2.4+

``` source
@MainActor
func performCommand(for keyCommand: UIKeyCommand) -> Bool
```

## Parameters 

`keyCommand`  

The key command received by the first responder.

## Return Value

Returns `YES` if a command corresponding to the UIKeyCommand was found and performed, `NO` otherwise.

## Discussion

This method checks for a command corresponding to the provided doc://com.apple.documentation/documentation/uikit/uikit/uikeycommand and performs it, if available. The app should use this method to perform any extension commands at an appropriate time in the app’s responder object that handles the performCommand(for:) action.

