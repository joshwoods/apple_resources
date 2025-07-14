

- UIKit
-  UIAppearance 

Protocol

# UIAppearance

A collection of methods that gives you access to the appearance proxy for a class.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
protocol UIAppearance : NSObjectProtocol
```

## Overview

You can customize the appearance of instances of a class by sending appearance-modification messages to the class’s appearance proxy.

Note

iOS applies appearance changes when a view enters a window, but it doesn’t change the appearance of a view that’s already in a window. To change the appearance of a view that’s currently in a window, remove the view from the view hierarchy and then put it back.

There are two ways to customize appearance for objects: for all instances, and for instances contained within an instance of a container class.

To customize the appearance of all instances of a class, use appearance() to get the appearance proxy for the class. For example, to modify the bar background tint color for all instances of UINavigationBar:

```
UINavigationBar.appearance().barTintColor = navBarTintColor
```

To customize the appearances for instances of a class when contained within an instance of a container class, or instances in a hierarchy, use appearanceWhenContainedIn: to get the appearance proxy for the class. For example, to modify the appearance of bar buttons, based on the object that contains the navigation bar:

```
let navigationBarAppearance =
UINavigationBar.appearance(whenContainedInInstancesOf: [UINavigationController.self])
navigationBarAppearance.setBackgroundImage(navBarBackgroundImage, for: .any, barMetrics: .default)

let barButtonNavigationBarAppearance =
UIBarButtonItem.appearance(whenContainedInInstancesOf: [UINavigationBar.self])
barButtonNavigationBarAppearance.setBackgroundImage(barButtonNavBarImage, for: .normal, barMetrics: .default)

let barButtonToolbarAppearance =
UIBarButtonItem.appearance(whenContainedInInstancesOf: [UIToolbar.self])
barButtonToolbarAppearance.setBackgroundImage(barButtonToolbarImage, for: .normal, barMetrics: .default)
```

In any given view hierarchy, the outermost appearance proxy wins. Specificity (depth of the chain) is the tie-breaker. In other words, the containment statement in appearanceWhenContainedIn: is treated as a partial ordering. Given a concrete ordering (actual subview hierarchy), UIKit selects the partial ordering that’s the first unique match when reading the actual hierarchy from the window down.

You can further refine which instances of a class will have their appearance customized by specifying a trait collection. Use the appearance(for:) and appearanceForTraitCollection:whenContainedIn: methods to retrieve the proxy for a class with the specified trait collection.

To support appearance customization, a class must conform to the UIAppearanceContainer protocol and relevant accessor methods must be marked with UI_APPEARANCE_SELECTOR.

## Topics

### Working with the appearance proxy

static func appearance() -> Self

Returns the appearance proxy for the receiver.

**Required**

static func appearance(for: UITraitCollection) -> Self

Returns the appearance proxy for the receiver that has the passed trait collection.

**Required**

static func appearance(whenContainedInInstancesOf: [any UIAppearanceContainer.Type]) -> Self

Returns the appearance proxy for the object when it’s contained in the hierarchy the specified classes describe.

**Required**

static func appearance(for: UITraitCollection, whenContainedInInstancesOf: [any UIAppearanceContainer.Type]) -> Self

Returns the appearance proxy for the object when it’s contained in the hierarchy the specified classes describe and has the specified trait collection.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- UIActionSheet
- UIActivityIndicatorView
- UIAlertView
- UIBarButtonItem
- UIBarItem
- UIButton
- UICalendarView
- UICollectionReusableView
- UICollectionView
- UICollectionViewCell
- UICollectionViewListCell
- UIColorWell
- UIContentUnavailableView
- UIControl
- UIDatePicker
- UIEventAttributionView
- UIImageView
- UIInputView
- UILabel
- UIListContentView
- UINavigationBar
- UIPageControl
- UIPasteControl
- UIPickerView
- UIPopoverBackgroundView
- UIProgressView
- UIRefreshControl
- UIScrollView
- UISearchBar
- UISearchTextField
- UISegmentedControl
- UISlider
- UIStackView
- UIStandardTextCursorView
- UIStepper
- UISwitch
- UITabBar
- UITabBarItem
- UITableView
- UITableViewCell
- UITableViewHeaderFooterView
- UITextField
- UITextView
- UIToolbar
- UIView
- UIVisualEffectView
- UIWebView
- UIWindow

## See Also

### Appearance proxies

protocol UIAppearanceContainer

A protocol that a class must adopt to allow appearance customization using the UIAppearance API.

