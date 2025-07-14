

- UIKit
-  UIAlertViewDelegate Deprecated

Protocol

# UIAlertViewDelegate

The interface for the delegate of an alert view object.

iOSiPadOSMac Catalyst

``` source
@MainActor
protocol UIAlertViewDelegate : NSObjectProtocol
```

Deprecated

Use UIAlertController instead.

## Overview

The delegate implements the button actions and any other custom behavior. Some of the methods defined in this protocol are optional.

If you add your own buttons or customize the behavior of an alert view, implement a delegate conforming to this protocol to handle the corresponding delegate messages. Use the delegate property of an alert view to specify one of your application objects as the delegate.

If you add your own buttons to an alert view, the delegate must implement the alertView(_:clickedButtonAt:) message to respond when those buttons are clicked; otherwise, your custom buttons do nothing. The alert view is automatically dismissed after the alertView(_:clickedButtonAt:) delegate method is invoked.

Optionally, you can implement the alertViewCancel(_:) method to take the appropriate action when the system cancels your alert view. If the delegate doesn’t implement this method, the default behavior is to simulate the user clicking the cancel button and closing the view.

You can also optionally augment the behavior of presenting and dismissing alert views using the methods in Customizing behavior.

## Topics

### Responding to actions

func alertView(UIAlertView, clickedButtonAt: Int)

Sent to the delegate when the user clicks a button on an alert view.

### Customizing behavior

func alertViewShouldEnableFirstOtherButton(UIAlertView) -> Bool

Sent to the delegate to determine whether the first non-cancel button in the alert should be enabled.

func willPresent(UIAlertView)

Sent to the delegate before a model view is presented to the user.

func didPresent(UIAlertView)

Sent to the delegate after an alert view is presented to the user.

func alertView(UIAlertView, willDismissWithButtonIndex: Int)

Sent to the delegate before an alert view is dismissed.

func alertView(UIAlertView, didDismissWithButtonIndex: Int)

Sent to the delegate after an alert view is dismissed from the screen.

### Canceling

func alertViewCancel(UIAlertView)

Sent to the delegate before an alert view is canceled.

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

protocol UIPopoverControllerDelegate

The interface for the delegate of a popover controller object.

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

