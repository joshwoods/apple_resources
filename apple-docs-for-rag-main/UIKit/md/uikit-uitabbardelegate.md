

- UIKit
-  UITabBarDelegate 

Protocol

# UITabBarDelegate

The UITabBarDelegate protocol defines optional methods for a delegate of a UITabBar object. The UITabBar class provides the ability for the user to reorder, remove, and add items to the tab bar; this process is referred to as customizing the tab bar. The tab bar delegate receives messages when customizing occurs.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
protocol UITabBarDelegate : NSObjectProtocol
```

## Overview

Send beginCustomizingItems(_:) to a UITabBar object to begin customizing. Implement the methods in Customizing tab bars to intervene while a user is customizing a tab bar. The customizing modal view is dismissed when the user taps the Done button on the modal view.

## Topics

### Customizing tab bars

func tabBar(UITabBar, willBeginCustomizing: [UITabBarItem])

Sent to the delegate before the customizing modal view is displayed.

func tabBar(UITabBar, didBeginCustomizing: [UITabBarItem])

Sent to the delegate after the customizing modal view is displayed.

func tabBar(UITabBar, willEndCustomizing: [UITabBarItem], changed: Bool)

Sent to the delegate before the customizing modal view is dismissed.

func tabBar(UITabBar, didEndCustomizing: [UITabBarItem], changed: Bool)

Sent to the delegate after the customizing modal view is dismissed.

func tabBar(UITabBar, didSelect: UITabBarItem)

Sent to the delegate when the user selects a tab bar item.

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- UITabBarController

## See Also

### Customizing the tab bar behavior

var delegate: (any UITabBarDelegate)?

The tab bar’s delegate object.

