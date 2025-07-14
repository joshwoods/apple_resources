

- AppKit
- NSResponder
-  performTextFinderAction(\_:) 

Instance Method

# performTextFinderAction(\_:)

Performs all find oriented actions.

macOS 10.7+

``` source
@MainActor
func performTextFinderAction(_ sender: Any?)
```

## Parameters 

`sender`  

The sender of the find action.

## Discussion

When an application performs a find action, it should send this message to the responder chain.

A responder of `performTextFinderAction:` is responsible for creating and owning an instance of `NSTextFinder`. Before any other messages are sent to the `NSTextFinder`, you should set its ‘client’ property to an object which implements the `NSTextFinderClient` protocol.

Note

Before OS X v10.7, the default action for these menu items was performFindPanelAction(_:). Whenever possible which you should update your implementation to use this new action.

