

- UIKit
- UISplitViewControllerDelegate
-  splitViewControllerSupportedInterfaceOrientations(\_:) 

Instance Method

# splitViewControllerSupportedInterfaceOrientations(\_:)

Asks the delegate to specify the interface orientations that the split view controller supports.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func splitViewControllerSupportedInterfaceOrientations(_ splitViewController: UISplitViewController) -> UIInterfaceOrientationMask
```

## Parameters 

`splitViewController`  

The split view controller.

## Return Value

The orientations that you want the specified split view controller to support. The value you return can be one or more of the UIInterfaceOrientationMask constants.

## Discussion

The split view controller calls this method to obtain the orientations that it supports. You can use this method to alter the set of orientations typically supported by a split view controller. If you don’t implement this method, the split view controller supports all orientations on iPad and all but the allButUpsideDown orientation on iPhone devices.

## See Also

### Related Documentation

var supportedInterfaceOrientations: UIInterfaceOrientationMask

The interface orientations that the view controller supports.

### Specifying the interface orientations

func splitViewControllerPreferredInterfaceOrientationForPresentation(UISplitViewController) -> UIInterfaceOrientation

Asks the delegate for the orientation to use when presenting the split view controller.

