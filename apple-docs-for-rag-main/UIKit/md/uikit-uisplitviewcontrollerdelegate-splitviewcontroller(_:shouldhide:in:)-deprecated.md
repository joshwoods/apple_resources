

- UIKit
- UISplitViewControllerDelegate
-  splitViewController(\_:shouldHide:in:) Deprecated

Instance Method

# splitViewController(\_:shouldHide:in:)

Asks the delegate whether the first view controller should be hidden for the specified orientation.

iOS 5.0–8.0DeprecatediPadOS 5.0–8.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
optional func splitViewController(
    _ svc: UISplitViewController,
    shouldHide vc: UIViewController,
    in orientation: UIInterfaceOrientation
) -> Bool
```

Deprecated

Orientation-related delegate methods are no longer supported.

## Parameters 

`svc`  

The split view controller that owns the first view controller.

`vc`  

The first view controller in the array of view controllers.

`orientation`  

The orientation being considered.

## Return Value

true if the view controller should be hidden in the specified orientation or false if it should be visible. If you do not implement this method, a value of true is assumed for portrait orientations and false is assumed for landscape orientations.

## Discussion

The split view controller calls this method only for the first child view controller in its array. The second view controller always remains visible regardless of the orientation.

Prior to iOS 5.0, the first view controller was always hidden in portrait orientations and always shown in landscape orientations. If you do not implement this method in your delegate object, that default behavior remains in effect.

## See Also

### Deprecated methods

func splitViewController(UISplitViewController, willHide: UIViewController, with: UIBarButtonItem, for: UIPopoverController)

Tells the delegate that the specified view controller is about to be hidden.

Deprecated

func splitViewController(UISplitViewController, willShow: UIViewController, invalidating: UIBarButtonItem)

Tells the delegate that the specified view controller is about to be shown again.

Deprecated

func splitViewController(UISplitViewController, popoverController: UIPopoverController, willPresent: UIViewController)

Tells the delegate that the hidden view controller is about to be displayed in a popover.

Deprecated

