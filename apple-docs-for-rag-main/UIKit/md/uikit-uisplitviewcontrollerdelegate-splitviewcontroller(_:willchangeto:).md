

- UIKit
- UISplitViewControllerDelegate
-  splitViewController(\_:willChangeTo:) 

Instance Method

# splitViewController(\_:willChangeTo:)

Tells the delegate that the display mode for the split view controller is about to change.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func splitViewController(
    _ svc: UISplitViewController,
    willChangeTo displayMode: UISplitViewController.DisplayMode
)
```

## Parameters 

`svc`  

The split view controller whose display mode is changing.

`displayMode`  

The new display mode that is about to be applied to the split view controller.

## Discussion

The split view controller calls this method when its display mode is about to change. Because changing the display mode usually means hiding or showing one of the child view controllers, you can implement this method and use it to add or remove the controls for showing the primary view controller.

## See Also

### Responding to display mode changes

func targetDisplayModeForAction(in: UISplitViewController) -> UISplitViewController.DisplayMode

Asks the delegate to provide the display mode to apply when a split view controller action occurs.

