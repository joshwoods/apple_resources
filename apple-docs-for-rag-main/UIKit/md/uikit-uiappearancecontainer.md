

- UIKit
-  UIAppearanceContainer 

Protocol

# UIAppearanceContainer

A protocol that a class must adopt to allow appearance customization using the UIAppearance API.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
protocol UIAppearanceContainer : NSObjectProtocol
```

## Overview

To participate in the appearance proxy API, tag appearance property accessor methods in your header with UI_APPEARANCE_SELECTOR.

Appearance property accessor methods must be of the form:

- Swift
- Objective-C

```
func propertyForAxis1(axis1: IntegerType, axis2: IntegerType, axisN: IntegerType) -> PropertyType
func setProperty(property: PropertyType, forAxis1 axis1: IntegerType, axis2: IntegerType)
```

```
- (PropertyType)propertyForAxis1:(IntegerType)axis1 axis2:(IntegerType)axis2 … axisN:(IntegerType)axisN;
- (void)setProperty:(PropertyType)property forAxis1:(IntegerType)axis1 axis2:(IntegerType)axis2 … axisN:(IntegerType)axisN;
```

You may have no axes or as many as you like for any property.

The property type may be any standard iOS type: `id`, NSInteger, NSUInteger, CGFloat, CGPoint, CGSize, CGRect, UIEdgeInsets or UIOffset. Axis parameter values must be either NSInteger or NSUInteger. UIKit throws an exception if other types are used in the axes.

For example, UIBarButtonItem defines these methods:

- setTitlePositionAdjustment(_:for:)

- backButtonBackgroundImage(for:barMetrics:)

- setBackButtonBackgroundImage(_:for:barMetrics:)

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- UIActionSheet
- UIActivityIndicatorView
- UIActivityViewController
- UIAlertController
- UIAlertView
- UIButton
- UICalendarView
- UICloudSharingController
- UICollectionReusableView
- UICollectionView
- UICollectionViewCell
- UICollectionViewController
- UICollectionViewListCell
- UIColorPickerViewController
- UIColorWell
- UIContentUnavailableView
- UIControl
- UIDatePicker
- UIDocumentBrowserViewController
- UIDocumentMenuViewController
- UIDocumentPickerExtensionViewController
- UIDocumentPickerViewController
- UIDocumentViewController
- UIEventAttributionView
- UIFontPickerViewController
- UIImagePickerController
- UIImageView
- UIInputView
- UIInputViewController
- UILabel
- UIListContentView
- UINavigationBar
- UINavigationController
- UIPageControl
- UIPageViewController
- UIPasteControl
- UIPickerView
- UIPopoverBackgroundView
- UIPopoverController
- UIPopoverPresentationController
- UIPresentationController
- UIProgressView
- UIReferenceLibraryViewController
- UIRefreshControl
- UIScrollView
- UISearchBar
- UISearchContainerViewController
- UISearchController
- UISearchTextField
- UISegmentedControl
- UISheetPresentationController
- UISlider
- UISplitViewController
- UIStackView
- UIStandardTextCursorView
- UIStepper
- UISwitch
- UITabBar
- UITabBarController
- UITableView
- UITableViewCell
- UITableViewController
- UITableViewHeaderFooterView
- UITextField
- UITextFormattingViewController
- UITextView
- UIToolbar
- UIVideoEditorController
- UIView
- UIViewController
- UIVisualEffectView
- UIWebView
- UIWindow

## See Also

### Appearance proxies

protocol UIAppearance

A collection of methods that gives you access to the appearance proxy for a class.

