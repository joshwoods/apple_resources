

- UIKit
- UISplitViewControllerDelegate
-  targetDisplayModeForAction(in:) 

Instance Method

# targetDisplayModeForAction(in:)

Asks the delegate to provide the display mode to apply when a split view controller action occurs.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func targetDisplayModeForAction(in svc: UISplitViewController) -> UISplitViewController.DisplayMode
```

## Parameters 

`svc`  

The split view controller whose action may be triggered. Use this object to obtain the current display mode and configuration of the split view interface.

## Return Value

The display mode to apply to the split view controller when the user performs specific actions.

## Discussion

This delegate method only applies to classic split view interfaces. For more information, see Split view styles.

The split view controller calls this method to determine which display mode to apply to itself in response to user-initiated actions. The split view controller has a built-in gesture recognizer that changes the current display mode. It also provides a bar button item from its displayModeButtonItem property that changes the display mode. The gesture recognizer is enabled using the presentsWithGesture property of the split view controller. Apps must incorporate the bar button item into their interface.

Implement this method if you want to specify which display mode to apply to the split view controller in response to the user actions. The split view controller calls this method to obtain an updated value for the gesture and bar button item. If you do not implement this method or if your method returns UISplitViewController.DisplayMode.automatic, the split view controller applies its own heuristics to determine which mode to apply when the next action is triggered. You cannot specify different display modes for the gesture and bar button item.

## See Also

### Responding to display mode changes

func splitViewController(UISplitViewController, willChangeTo: UISplitViewController.DisplayMode)

Tells the delegate that the display mode for the split view controller is about to change.

