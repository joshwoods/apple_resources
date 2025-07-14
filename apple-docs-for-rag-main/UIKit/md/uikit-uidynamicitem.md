

- UIKit
-  UIDynamicItem 

Protocol

# UIDynamicItem

A set of methods that can make a custom object eligible to participate in UIKit Dynamics.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
protocol UIDynamicItem : NSObjectProtocol
```

## Overview

Starting in iOS 7, the UIView and UICollectionViewLayoutAttributes classes implement this protocol.

## Topics

### Participating in dynamic animation

var bounds: CGRect

Called when a dynamic animator needs the bounds of the dynamic item.

**Required**

var center: CGPoint

The center point of the dynamic item.

**Required**

var transform: CGAffineTransform

The rotation of the dynamic item.

**Required**

var collisionBoundsType: UIDynamicItemCollisionBoundsType

The type of collision bounds associated with the item.

var collisionBoundingPath: UIBezierPath

The path-based shape to use for the collision bounds.

### Constants

enum UIDynamicItemCollisionBoundsType

Constants that indicate the shape of the item’s collision bounds.

## Relationships

### Inherits From

- NSObjectProtocol

### Inherited By

- NSCollectionLayoutVisibleItem

### Conforming Types

- UIActionSheet
- UIActivityIndicatorView
- UIAlertView
- UIButton
- UICalendarView
- UICollectionReusableView
- UICollectionView
- UICollectionViewCell
- UICollectionViewLayoutAttributes
- UICollectionViewListCell
- UIColorWell
- UIContentUnavailableView
- UIControl
- UIDatePicker
- UIDynamicItemGroup
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

### Dynamic Items

class UIDynamicItemBehavior

A base dynamic animation configuration for one or more dynamic items.

class UIDynamicItemGroup

A dynamic item that comprises multiple other dynamic items.

