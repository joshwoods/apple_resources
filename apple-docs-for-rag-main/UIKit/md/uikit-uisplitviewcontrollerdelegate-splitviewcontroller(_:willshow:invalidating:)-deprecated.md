

- UIKit
- UISplitViewControllerDelegate
-  splitViewController(\_:willShow:invalidating:) Deprecated

Instance Method

# splitViewController(\_:willShow:invalidating:)

Tells the delegate that the specified view controller is about to be shown again.

iOS 2.0–8.0DeprecatediPadOS 2.0–8.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
optional func splitViewController(
    _ svc: UISplitViewController,
    willShow aViewController: UIViewController,
    invalidating barButtonItem: UIBarButtonItem
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

The button used to display the view controller while it was hidden.

## Discussion

When the view controller rotates from a portrait to landscape orientation, it shows its hidden view controller once more. If you added the specified button to your toolbar to facilitate the display of the hidden view controller in a popover, you must implement this method and use it to remove that button.

## See Also

### Deprecated methods

func splitViewController(UISplitViewController, shouldHide: UIViewController, in: UIInterfaceOrientation) -> Bool

Asks the delegate whether the first view controller should be hidden for the specified orientation.

Deprecated

func splitViewController(UISplitViewController, willHide: UIViewController, with: UIBarButtonItem, for: UIPopoverController)

Tells the delegate that the specified view controller is about to be hidden.

Deprecated

func splitViewController(UISplitViewController, popoverController: UIPopoverController, willPresent: UIViewController)

Tells the delegate that the hidden view controller is about to be displayed in a popover.

Deprecated

