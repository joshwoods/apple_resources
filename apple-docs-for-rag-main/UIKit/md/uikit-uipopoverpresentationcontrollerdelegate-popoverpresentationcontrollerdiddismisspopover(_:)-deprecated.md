

- UIKit
- UIPopoverPresentationControllerDelegate
-  popoverPresentationControllerDidDismissPopover(\_:) Deprecated

Instance Method

# popoverPresentationControllerDidDismissPopover(\_:)

Tells the delegate that the popover was dismissed.

iOS 8.0–13.0DeprecatediPadOS 8.0–13.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
optional func popoverPresentationControllerDidDismissPopover(_ popoverPresentationController: UIPopoverPresentationController)
```

## Parameters 

`popoverPresentationController`  

The popover presentation controller that is managing the popover interface.

## Discussion

The popover presentation controller calls this method after dismissing the popover to let you know that it is no longer onscreen. The presentation controller calls this method only in response to user actions. It does not call this method if you dismiss the popover programmatically.

Use this method to incorporate any changes from the popover’s content view controller back into your app.

## See Also

### Presenting and dismissing the popover

func prepareForPopoverPresentation(UIPopoverPresentationController)

Notifies the delegate that the popover is about to be presented.

func popoverPresentationControllerShouldDismissPopover(UIPopoverPresentationController) -> Bool

Asks the delegate if the popover should be dismissed.

Deprecated

