

- UIKit
-  UIPopoverPresentationControllerDelegate 

Protocol

# UIPopoverPresentationControllerDelegate

The interface for a popover presentation delegate, which lets you customize the behavior of a popover-based presentation.

iOSiPadOSMac CatalystvisionOS

``` source
@MainActor
protocol UIPopoverPresentationControllerDelegate : UIAdaptivePresentationControllerDelegate
```

## Overview

A popover presentation controller notifies your delegate at appropriate points during the presentation process. You can use the delegate methods to customize this process and respond to changes dynamically.

After defining an object that adopts this protocol, assign that object to the delegate property of a UIPopoverPresentationController object. You must present a view controller using the UIModalPresentationStyle.popover style before you can obtain such an object. For more information about popover presentation controllers, see UIPopoverPresentationController.

## Topics

### Presenting and dismissing the popover

func prepareForPopoverPresentation(UIPopoverPresentationController)

Notifies the delegate that the popover is about to be presented.

func popoverPresentationControllerShouldDismissPopover(UIPopoverPresentationController) -> Bool

Asks the delegate if the popover should be dismissed.

Deprecated

func popoverPresentationControllerDidDismissPopover(UIPopoverPresentationController)

Tells the delegate that the popover was dismissed.

Deprecated

### Repositioning the popover

func popoverPresentationController(UIPopoverPresentationController, willRepositionPopoverTo: UnsafeMutablePointer&lt;CGRect>, in: AutoreleasingUnsafeMutablePointer&lt;UIView>)

Tells the delegate that UIKit needs to reposition the popover’s location.

## Relationships

### Inherits From

- NSObjectProtocol
- UIAdaptivePresentationControllerDelegate

## See Also

### Customizing the popover behavior

var delegate: (any UIPopoverPresentationControllerDelegate)?

The delegate that handles popover-related messages.

