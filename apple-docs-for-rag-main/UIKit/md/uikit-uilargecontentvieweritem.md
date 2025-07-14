

- UIKit
-  UILargeContentViewerItem 

Protocol

# UILargeContentViewerItem

Methods that provide details about how to display your custom content in the large content viewer.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
protocol UILargeContentViewerItem : NSObjectProtocol
```

## Topics

### Integrating with the large content viewer

var showsLargeContentViewer: Bool

A Boolean value that indicates whether or not to show the item in the large content viewer.

**Required**

### Configuring display properties

var largeContentTitle: String?

A string that describes an item to display in the large content viewer.

**Required**

var largeContentImage: UIImage?

An image that represents an item to display in the large content viewer.

**Required**

var largeContentImageInsets: UIEdgeInsets

Insets to adjust the position of the item’s image so it appears visually centered in the large content viewer.

**Required**

var scalesLargeContentImage: Bool

A Boolean value that indicates whether the view scales the item’s image to a larger size or not.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

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

### Content viewer

class UILargeContentViewerInteraction

An interaction that enables a gesture to present the large content viewer for cases when supporting the largest dynamic type sizes isn’t appropriate.

protocol UILargeContentViewerInteractionDelegate

An object that customizes the behavior of the large content viewer interactions.

