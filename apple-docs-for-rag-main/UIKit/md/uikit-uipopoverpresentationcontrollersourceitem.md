

- UIKit
-  UIPopoverPresentationControllerSourceItem 

Protocol

# UIPopoverPresentationControllerSourceItem

A type that can be an anchor for a popover presentation controller.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
protocol UIPopoverPresentationControllerSourceItem : NSObjectProtocol
```

## Topics

### Instance Methods

func frame(in: UIView) -> CGRect?

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- NSUIViewToolbarItem
- UIActionSheet
- UIActivityIndicatorView
- UIAlertView
- UIBarButtonItem
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
- UIFocusGuide
- UIImageView
- UIInputView
- UIKeyboardLayoutGuide
- UILabel
- UILayoutGuide
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
- UISearchTab
- UISearchTextField
- UISegmentedControl
- UISlider
- UIStackView
- UIStandardTextCursorView
- UIStepper
- UISwitch
- UITab
- UITabBar
- UITabBarItem
- UITabGroup
- UITableView
- UITableViewCell
- UITableViewHeaderFooterView
- UITextField
- UITextView
- UIToolbar
- UITrackingLayoutGuide
- UIView
- UIVisualEffectView
- UIWebView
- UIWindow

## See Also

### Specifying the popover’s anchor point

var sourceItem: (any UIPopoverPresentationControllerSourceItem)?

The item on which to anchor the popover.

var sourceView: UIView?

The view containing the anchor rectangle for the popover.

var sourceRect: CGRect

The area in the source view in which you anchor the popover.

var barButtonItem: UIBarButtonItem?

The bar button item on which to anchor the popover.

Deprecated

