

- UIKit
- UIPopoverPresentationControllerDelegate
-  popoverPresentationControllerShouldDismissPopover(\_:) Deprecated

Instance Method

# popoverPresentationControllerShouldDismissPopover(\_:)

Asks the delegate if the popover should be dismissed.

iOS 8.0–13.0DeprecatediPadOS 8.0–13.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
optional func popoverPresentationControllerShouldDismissPopover(_ popoverPresentationController: UIPopoverPresentationController) -> Bool
```

## Parameters 

`popoverPresentationController`  

The popover presentation controller that is managing the popover interface.

## Return Value

true if the popover should be dismissed or false if it should not.

## Discussion

The popover presentation controller calls this method in response to user-initiated attempts to dismiss the popover. It is not called when you dismiss the popover programmatically using the dismissModalViewControllerAnimated: method.

If you do not implement this method in your delegate, the default return value is assumed to be true.

## See Also

### Presenting and dismissing the popover

func prepareForPopoverPresentation(UIPopoverPresentationController)

Notifies the delegate that the popover is about to be presented.

func popoverPresentationControllerDidDismissPopover(UIPopoverPresentationController)

Tells the delegate that the popover was dismissed.

Deprecated

