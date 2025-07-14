

- UIKit
-  UIPopoverControllerDelegate Deprecated

Protocol

# UIPopoverControllerDelegate

The interface for the delegate of a popover controller object.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
protocol UIPopoverControllerDelegate : NSObjectProtocol
```

Deprecated

In iOS 9 and later, a popover is implemented as a UIViewController presentation. To create a popover, use UIPopoverPresentationController and specify the UIModalPresentationStyle.popover style.

## Overview

Popover controllers notify their delegate whenever user interactions would cause the dismissal of the popover and, in some cases, give the user a chance to prevent that dismissal.

For more information about the UIPopoverController class, see UIPopoverController.

## Topics

### Responding to popover position changes

func popoverController(UIPopoverController, willRepositionPopoverTo: UnsafeMutablePointer&lt;CGRect>, in: AutoreleasingUnsafeMutablePointer&lt;UIView>)

Tells the delegate that the popover controller needs to change the popover’s location in its view.

### Managing the popover’s dismissal

func popoverControllerShouldDismissPopover(UIPopoverController) -> Bool

Asks the delegate if the popover should be dismissed.

func popoverControllerDidDismissPopover(UIPopoverController)

Tells the delegate that the popover was dismissed.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Deprecated protocols

protocol UIAccelerometerDelegate

The interface for receiving acceleration-related data from the system.

Deprecated

protocol UIActionSheetDelegate

The interface for the delegate of an action sheet object.

Deprecated

protocol UIAlertViewDelegate

The interface for the delegate of an alert view object.

Deprecated

protocol UISearchDisplayDelegate

The interface for the delegate of a search display controller.

Deprecated

protocol UIViewControllerPreviewing

A set of methods that define the interface for configuring a previewing view controller on devices that support 3D Touch.

Deprecated

protocol UIViewControllerPreviewingDelegate

A set of methods used by the delegate to respond, with a preview view controller and a commit view controller, to the user pressing a view object on the screen of a device that supports 3D Touch.

Deprecated

