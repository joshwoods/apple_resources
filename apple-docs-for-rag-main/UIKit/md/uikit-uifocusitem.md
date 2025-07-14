

- UIKit
-  UIFocusItem 

Protocol

# UIFocusItem

An object that can become focused.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
protocol UIFocusItem : UIFocusEnvironment
```

## Overview

An object that conforms to the UIFocusItem protocol is capable of participating in the focus system; further, only UIFocusItem objects can be focused.

Even when an object that conforms to UIFocusItem isn’t currently focusable, it may still have an effect on the focus system. For example, items that aren’t focusable, but that completely obscure other items, may prevent those other items from being focusable, because they aren’t visible to the user. Also, because UIFocusItem conforms to UIFocusEnvironment, items that aren’t focusable may still affect the focus behavior of items they contain, or react to focus updates.

## Topics

### Determining focusability

var canBecomeFocused: Bool

A Boolean value that indicates whether the item can become focused.

**Required**

var isFocused: Bool

A Boolean value that indicates whether the item is currently focused.

### Retrieving the item frame

var frame: CGRect

The geometric frame of the item.

**Required**

### Determining the focus priority

var focusGroupPriority: UIFocusGroupPriority

The importance of the item within a focus group, used by the focus system to determine the group’s primary item.

struct UIFocusGroupPriority

The importance of an item within a focus group, used by the focus system to determine the group’s primary item.

### Providing movement hints

func didHintFocusMovement(UIFocusMovementHint)

Indicates to the currently focused item that focus movement might occur.

class UIFocusMovementHint

Provides movement hint information for the focused item.

### Indicating focus visually

var focusEffect: UIFocusEffect?

The visual effect to apply when the item becomes focused.

### Working with transparent items

var isTransparentFocusItem: Bool

Indicates if the focus item is transparent, which allows items behind it to become focused.

### Instance Properties

var focusItemDeferralMode: UIFocusItemDeferralMode

## Relationships

### Inherits From

- NSObjectProtocol
- UIFocusEnvironment

### Conforming Types

- UIActionSheet
- UIActivityIndicatorView
- UIAlertView
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

### Focus interactions

Navigating an app’s user interface using a keyboard

Navigate between user interface elements using a keyboard and focusable UI elements in iPad apps and apps built with Mac Catalyst.

About focus interactions for Apple TV

Design and implement intuitive control schemes for menus and interactive user interface layouts.

Adding user-focusable elements to a tvOS app

Create intuitive and easily manipulated user-interactive controls for your tvOS app.

protocol UIFocusEnvironment

A set of methods that define the focus behavior for a branch of the view hierarchy.

class UIFocusSystem

Queries and reevaluates the currently focused item.

class UIFocusUpdateContext

An object that provides information relevant to a specific focus update from one view to another.

class UIFocusMovementHint

Provides movement hint information for the focused item.

protocol UIFocusItemContainer

The container responsible for providing geometric context to focus items within a given focus environment.

protocol UIFocusItemScrollableContainer

A type of focus item container that supports automatic scrolling of focusable content.

struct UIFocusGroupPriority

The importance of an item within a focus group, used by the focus system to determine the group’s primary item.

