

- UIKit
- UIPopoverControllerDelegate
-  popoverControllerShouldDismissPopover(\_:) Deprecated

Instance Method

# popoverControllerShouldDismissPopover(\_:)

Asks the delegate if the popover should be dismissed.

iOS 3.2–9.0DeprecatediPadOS 3.2–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOSDeprecated

``` source
@MainActor
optional func popoverControllerShouldDismissPopover(_ popoverController: UIPopoverController) -> Bool
```

## Parameters 

`popoverController`  

The popover controller to be dismissed.

## Return Value

true if the popover should be dismissed or false if it should remain visible.

## Discussion

This method is called in response to user-initiated attempts to dismiss the popover. It is not called when you dismiss the popover using the dismiss(animated:) method of the popover controller.

If you do not implement this method in your delegate, the default return value is assumed to be true.

## See Also

### Managing the popover’s dismissal

func popoverControllerDidDismissPopover(UIPopoverController)

Tells the delegate that the popover was dismissed.

Deprecated

