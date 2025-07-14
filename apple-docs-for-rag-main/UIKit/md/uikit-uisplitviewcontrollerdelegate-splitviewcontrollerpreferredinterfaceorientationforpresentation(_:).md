

- UIKit
- UISplitViewControllerDelegate
-  splitViewControllerPreferredInterfaceOrientationForPresentation(\_:) 

Instance Method

# splitViewControllerPreferredInterfaceOrientationForPresentation(\_:)

Asks the delegate for the orientation to use when presenting the split view controller.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func splitViewControllerPreferredInterfaceOrientationForPresentation(_ splitViewController: UISplitViewController) -> UIInterfaceOrientation
```

## Parameters 

`splitViewController`  

The split view controller that is about to be presented onscreen.

## Return Value

The orientation to use when first displaying the split view controller.

## Discussion

UIKit calls this method to determine which orientation your app prefers when presenting the specified split view controller. You can use this method to specify the orientation that you think is best when first displaying the split view controller. The orientation you specify can be different from the current device orientation. After presentation, the system may rotate the split view controller as appropriate to one of its other supported interface orientations.

If you do not implement this method, the system presents the view controller using the current orientation of the status bar.

## See Also

### Related Documentation

var preferredInterfaceOrientationForPresentation: UIInterfaceOrientation

The interface orientation to use when presenting the view controller.

### Specifying the interface orientations

func splitViewControllerSupportedInterfaceOrientations(UISplitViewController) -> UIInterfaceOrientationMask

Asks the delegate to specify the interface orientations that the split view controller supports.

