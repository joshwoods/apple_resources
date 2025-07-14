

- AppKit
- NSWritingToolsCoordinator
- NSWritingToolsCoordinator.Delegate
-  writingToolsCoordinator(\_:willChangeTo:completion:) 

Instance Method

# writingToolsCoordinator(\_:willChangeTo:completion:)

Notifies your delegate of relevant state changes when Writing Tools is running in your view.

macOS 15.2+

``` source
optional func writingToolsCoordinator(
    _ writingToolsCoordinator: NSWritingToolsCoordinator,
    willChangeTo newState: NSWritingToolsCoordinator.State,
    completion: @escaping () -> Void
)
```

``` source
optional func writingToolsCoordinator(
    _ writingToolsCoordinator: NSWritingToolsCoordinator,
    willChangeTo newState: NSWritingToolsCoordinator.State
) async
```

## Parameters 

`writingToolsCoordinator`  

The coordinator object providing information to your custom view.

`completion`  

A handler to execute when your delegate finishes processing the change of state. The handler has no parameters or return value. You must call this handler at some point during the implementation of your method.

## Mentioned in 

Adding Writing Tools support to a custom AppKit view

## Discussion

Use state transitions to perform actions related to your view or text storage. When Writing Tools is active, it updates its state to indicate what task it’s currently performing. Writing Tools starts in the NSWritingToolsCoordinator.State.inactive state and moves to other states as it presents UI and starts interacting with your view’s content. For example, it moves to the `NSWritingToolsCoordinator/State/interactiveUpdating` state when it’s making changes to your view’s text storage.

