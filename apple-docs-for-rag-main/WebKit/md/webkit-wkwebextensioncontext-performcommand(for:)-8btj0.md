

- WebKit
- WKWebExtensionContext
-  performCommand(for:) 

Instance Method

# performCommand(for:)

Performs the command associated with the given event.

macOS 15.4+

``` source
@MainActor
func performCommand(for event: NSEvent) -> Bool
```

## Parameters 

`event`  

The event representing the user input.

## Return Value

Returns `YES` if a command corresponding to the event was found and performed, `NO` otherwise.

## Discussion

This method checks for a command corresponding to the provided event and performs it, if available. The app should use this method to perform any extension commands at an appropriate time in the app’s event handling, like in sendEvent(_:) of NSApplication or sendEvent(_:) of NSWindow subclasses.

