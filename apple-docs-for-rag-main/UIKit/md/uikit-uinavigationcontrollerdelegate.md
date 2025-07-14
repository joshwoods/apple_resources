

- UIKit
-  UINavigationControllerDelegate 

Protocol

# UINavigationControllerDelegate

The interface for an object that serves as a navigation controller’s delegate.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
protocol UINavigationControllerDelegate : NSObjectProtocol
```

## Overview

Use a navigation controller delegate (a custom object that implements this protocol) to modify behavior when a view controller is pushed or popped from the navigation stack of a UINavigationController object.

## Topics

### Responding to a view controller being shown

func navigationController(UINavigationController, willShow: UIViewController, animated: Bool)

Notifies the delegate before the navigation controller displays a view controller’s view and navigation item properties.

func navigationController(UINavigationController, didShow: UIViewController, animated: Bool)

Notifies the delegate after the navigation controller displays a view controller’s view and navigation item properties.

### Supporting custom transition animations

func navigationController(UINavigationController, animationControllerFor: UINavigationController.Operation, from: UIViewController, to: UIViewController) -> (any UIViewControllerAnimatedTransitioning)?

Allows the delegate to return a noninteractive animator object for use during view controller transitions.

func navigationController(UINavigationController, interactionControllerFor: any UIViewControllerAnimatedTransitioning) -> (any UIViewControllerInteractiveTransitioning)?

Allows the delegate to return an interactive animator object for use during view controller transitions.

func navigationControllerPreferredInterfaceOrientationForPresentation(UINavigationController) -> UIInterfaceOrientation

Returns the preferred orientation for presentation of the navigation controller, as determined by the delegate.

func navigationControllerSupportedInterfaceOrientations(UINavigationController) -> UIInterfaceOrientationMask

Returns the complete set of supported interface orientations for the navigation controller, as determined by the delegate.

### Constants

enum Operation

Constants that define the type of navigation controller transitions that can occur.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Customizing the navigation interface behavior

var delegate: (any UINavigationControllerDelegate)?

The delegate of the navigation controller object.

