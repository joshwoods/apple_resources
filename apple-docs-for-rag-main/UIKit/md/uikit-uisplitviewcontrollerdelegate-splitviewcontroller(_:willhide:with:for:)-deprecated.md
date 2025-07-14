

- UIKit
- UISplitViewControllerDelegate
-  splitViewController(\_:willHide:with:for:) Deprecated

Instance Method

# splitViewController(\_:willHide:with:for:)

Tells the delegate that the specified view controller is about to be hidden.

iOS 2.0–8.0DeprecatediPadOS 2.0–8.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
optional func splitViewController(
    _ svc: UISplitViewController,
    willHide aViewController: UIViewController,
    with barButtonItem: UIBarButtonItem,
    for pc: UIPopoverController
)
```

Deprecated

Implement the splitViewController(_:willChangeTo:) method instead.

## Parameters 

`svc`  

The split view controller that owns the specified view controller.

`aViewController`  

The view controller being hidden.

`barButtonItem`  

A button you can add to your toolbar.

`pc`  

The popover controller that uses taps in `barButtonItem` to display the specified view controller.

## Discussion

When the split view controller rotates from a landscape to portrait orientation, it typically hides one of its view controllers. When that happens, it calls this method to coordinate the addition of a button to the toolbar (or navigation bar) of the remaining custom view controller. If you want the soon-to-be hidden view controller to be displayed in a popover, you must implement this method and use it to add the specified button to your interface.

## See Also

### Deprecated methods

func splitViewController(UISplitViewController, shouldHide: UIViewController, in: UIInterfaceOrientation) -> Bool

Asks the delegate whether the first view controller should be hidden for the specified orientation.

Deprecated

func splitViewController(UISplitViewController, willShow: UIViewController, invalidating: UIBarButtonItem)

Tells the delegate that the specified view controller is about to be shown again.

Deprecated

func splitViewController(UISplitViewController, popoverController: UIPopoverController, willPresent: UIViewController)

Tells the delegate that the hidden view controller is about to be displayed in a popover.

Deprecated

