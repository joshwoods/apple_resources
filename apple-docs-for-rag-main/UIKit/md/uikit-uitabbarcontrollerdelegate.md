

- UIKit
-  UITabBarControllerDelegate 

Protocol

# UITabBarControllerDelegate

A set of methods you implement to customize the behavior of a tab bar.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
protocol UITabBarControllerDelegate : NSObjectProtocol
```

## Mentioned in 

Elevating your iPad app with a tab bar and sidebar

## Overview

You use the UITabBarControllerDelegate protocol when you want to augment the behavior of a tab bar. In particular, you can use it to determine whether specific tabs should be selected, to perform actions after a tab is selected, or to perform actions before or after the user customizes the order of the tabs. After implementing these methods in your custom object, you should then assign that object to the delegate property of the corresponding UITabBarController object.

All of the methods in this protocol are optional. For more information on how to use and configure tab bar controllers and their delegates, see View Controller Programming Guide for iOS.

## Topics

### Managing tab bar selections

func tabBarController(UITabBarController, shouldSelect: UIViewController) -> Bool

Asks the delegate whether the specified view controller should be made active.

func tabBarController(UITabBarController, didSelect: UIViewController)

Tells the delegate that the user selected an item in the tab bar.

### Managing tab bar customizations

func tabBarController(UITabBarController, willBeginCustomizing: [UIViewController])

Tells the delegate that the tab bar customization sheet is about to be displayed.

func tabBarController(UITabBarController, willEndCustomizing: [UIViewController], changed: Bool)

Tells the delegate that the tab bar customization sheet is about to be dismissed.

func tabBarController(UITabBarController, didEndCustomizing: [UIViewController], changed: Bool)

Tells the delegate that the tab bar customization sheet was dismissed.

### Overriding view rotation settings

func tabBarControllerSupportedInterfaceOrientations(UITabBarController) -> UIInterfaceOrientationMask

Called to allow the delegate to provide the complete set of supported interface orientations for the tab bar controller.

func tabBarControllerPreferredInterfaceOrientationForPresentation(UITabBarController) -> UIInterfaceOrientation

Called to allow the delegate to provide the preferred orientation for presentation of the tab bar controller.

### Supporting custom tab bar transition animations

func tabBarController(UITabBarController, animationControllerForTransitionFrom: UIViewController, to: UIViewController) -> (any UIViewControllerAnimatedTransitioning)?

Called to allow the delegate to return a UIViewControllerAnimatedTransitioning delegate object for use during a noninteractive tab bar view controller transition.

func tabBarController(UITabBarController, interactionControllerFor: any UIViewControllerAnimatedTransitioning) -> (any UIViewControllerInteractiveTransitioning)?

Called to allow the delegate to return a UIViewControllerInteractiveTransitioning delegate object for use during an animated tab bar transition.

### Instance Methods

func tabBarController(UITabBarController, didSelectTab: UITab, previousTab: UITab?)

func tabBarController(UITabBarController, displayOrderDidChangeFor: UITabGroup)

func tabBarController(UITabBarController, displayedViewControllersFor: UITab, proposedViewControllers: [UIViewController]) -> [UIViewController]

func tabBarController(UITabBarController, shouldSelectTab: UITab) -> Bool

func tabBarController(UITabBarController, tab: UITab, acceptItemsFrom: any UIDropSession)

func tabBarController(UITabBarController, tab: UITab, operationForAcceptingItemsFrom: any UIDropSession) -> UIDropOperation

func tabBarController(UITabBarController, visibilityDidChangeFor: [UITab])

func tabBarControllerDidEndEditing(UITabBarController)

func tabBarControllerWillBeginEditing(UITabBarController)

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Customizing the tab bar behavior

var delegate: (any UITabBarControllerDelegate)?

The tab bar controller’s delegate object.

