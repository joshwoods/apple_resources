

- UIKit
-  UIAdaptivePresentationControllerDelegate 

Protocol

# UIAdaptivePresentationControllerDelegate

A set of methods that, in conjunction with a presentation controller, determine how to respond to trait changes in your app.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
protocol UIAdaptivePresentationControllerDelegate : NSObjectProtocol
```

## Overview

After implementing an object that conforms to this protocol, assign that object to the delegate property of an appropriate UIPresentationController object. Your delegate can suggest a new presentation style or an entirely new view controller for displaying content. For more information about using the delegate to respond to size class changes, see UIPresentationController.

## Topics

### Adapting the presentation style

func adaptivePresentationStyle(for: UIPresentationController, traitCollection: UITraitCollection) -> UIModalPresentationStyle

Asks the delegate for the presentation style to use when the specified set of traits are active.

func adaptivePresentationStyle(for: UIPresentationController) -> UIModalPresentationStyle

Asks the delegate for the new presentation style to use.

### Adapting the view controller

func presentationController(UIPresentationController, viewControllerForAdaptivePresentationStyle: UIModalPresentationStyle) -> UIViewController?

Asks the delegate for the view controller to display when adapting to the specified presentation style.

### Responding to adaptive transitions

func presentationController(UIPresentationController, willPresentWithAdaptiveStyle: UIModalPresentationStyle, transitionCoordinator: (any UIViewControllerTransitionCoordinator)?)

Notifies the delegate that an adaptivity-related transition is about to occur.

func presentationControllerDidAttemptToDismiss(UIPresentationController)

Notifies the delegate that a user-initiated attempt to dismiss a view was prevented.

func presentationControllerShouldDismiss(UIPresentationController) -> Bool

Asks the delegate for permission to dismiss the presentation.

func presentationControllerDidDismiss(UIPresentationController)

Notifies the delegate after a presentation is dismissed.

func presentationControllerWillDismiss(UIPresentationController)

Notifies the delegate before a presentation is dismissed.

### Preparing the adaptive presentation controller

func presentationController(UIPresentationController, prepare: UIPresentationController)

Provides an opportunity to configure the adaptive presentation controller after an adaptivity change.

## Relationships

### Inherits From

- NSObjectProtocol

### Inherited By

- UIPopoverPresentationControllerDelegate
- UISheetPresentationControllerDelegate

## See Also

### Adaptivity

Automatic trait tracking

Reduce the need to manually register for trait changes when you use traits within a method or closure that supports automatic trait tracking.

Responding to changing display modes on Apple TV

Change images and resources dynamically when the screen gamut on your device changes.

class UITraitCollection

A collection of data that represents the environment for an individual element in your app’s user interface.

protocol UITraitEnvironment

A set of methods that makes the iOS interface environment available to your app.

protocol UITraitChangeObservable

A type that calls your code in reaction to changes in the trait environment.

protocol UIMutableTraits

A mutable container of traits.

protocol UIContentContainer

A set of methods for adapting the contents of your view controllers to size and trait changes.

