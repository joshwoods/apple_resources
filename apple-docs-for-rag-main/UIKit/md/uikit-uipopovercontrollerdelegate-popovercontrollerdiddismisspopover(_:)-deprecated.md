

- UIKit
- UIPopoverControllerDelegate
-  popoverControllerDidDismissPopover(\_:) Deprecated

Instance Method

# popoverControllerDidDismissPopover(\_:)

Tells the delegate that the popover was dismissed.

iOS 3.2–9.0DeprecatediPadOS 3.2–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOSDeprecated

``` source
@MainActor
optional func popoverControllerDidDismissPopover(_ popoverController: UIPopoverController)
```

## Parameters 

`popoverController`  

The popover controller that was dismissed.

## Discussion

The popover controller does not call this method in response to programmatic calls to the dismiss(animated:) method. If you dismiss the popover programmatically, you should perform any cleanup actions immediately after calling the dismiss(animated:) method.

You can use this method to incorporate any changes from the popover’s content view controller back into your application. If you do not plan to use the object in the `popoverController` parameter again, it is safe to release it from this method.

## See Also

### Managing the popover’s dismissal

func popoverControllerShouldDismissPopover(UIPopoverController) -> Bool

Asks the delegate if the popover should be dismissed.

Deprecated

