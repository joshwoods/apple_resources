

- UIKit
- UIPopoverPresentationControllerDelegate
-  prepareForPopoverPresentation(\_:) 

Instance Method

# prepareForPopoverPresentation(\_:)

Notifies the delegate that the popover is about to be presented.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func prepareForPopoverPresentation(_ popoverPresentationController: UIPopoverPresentationController)
```

## Parameters 

`popoverPresentationController`  

The popover presentation controller that is about to display the popover.

## Discussion

Use this method to perform any last minute customizations of the popover appearance and behavior. At the time this method is called, the popover is not yet on the screen. You can use this method to modify the configuration of the popover presentation controller or perform any other actions that your app requires.

## See Also

### Presenting and dismissing the popover

func popoverPresentationControllerShouldDismissPopover(UIPopoverPresentationController) -> Bool

Asks the delegate if the popover should be dismissed.

Deprecated

func popoverPresentationControllerDidDismissPopover(UIPopoverPresentationController)

Tells the delegate that the popover was dismissed.

Deprecated

