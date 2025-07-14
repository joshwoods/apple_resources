

- UIKit
- UISplitViewControllerDelegate
-  splitViewController(\_:popoverController:willPresent:) Deprecated

Instance Method

# splitViewController(\_:popoverController:willPresent:)

Tells the delegate that the hidden view controller is about to be displayed in a popover.

iOS 2.0–8.0DeprecatediPadOS 2.0–8.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
optional func splitViewController(
    _ svc: UISplitViewController,
    popoverController pc: UIPopoverController,
    willPresent aViewController: UIViewController
)
```

Deprecated

Orientation-related delegate methods are no longer supported.

## Parameters 

`svc`  

The split view controller that owns the hidden view controller.

`pc`  

The popover controller that is about to display the view controller.

`aViewController`  

The view controller to be displayed in the popover.

## Discussion

The toolbar button you add to your user interface facilitates the display of the hidden view controller in response to user taps. When the user taps that button, the split view controller calls this method. You can use this method to perform any additional steps prior to displaying the currently hidden view controller.

## See Also

### Deprecated methods

func splitViewController(UISplitViewController, shouldHide: UIViewController, in: UIInterfaceOrientation) -> Bool

Asks the delegate whether the first view controller should be hidden for the specified orientation.

Deprecated

func splitViewController(UISplitViewController, willHide: UIViewController, with: UIBarButtonItem, for: UIPopoverController)

Tells the delegate that the specified view controller is about to be hidden.

Deprecated

func splitViewController(UISplitViewController, willShow: UIViewController, invalidating: UIBarButtonItem)

Tells the delegate that the specified view controller is about to be shown again.

Deprecated

