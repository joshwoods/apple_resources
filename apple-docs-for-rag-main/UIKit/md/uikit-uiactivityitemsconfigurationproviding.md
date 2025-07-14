

- UIKit
-  UIActivityItemsConfigurationProviding 

Protocol

# UIActivityItemsConfigurationProviding

An interface that provides a source for shareable content to fulfill user requests to share current content.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
protocol UIActivityItemsConfigurationProviding : NSObjectProtocol
```

## Overview

The user can share content from your app in a number of ways:

- Ask Siri to “share this” on an iOS device.

- Click an NSSharingServicePickerToolbarItem in the toolbar of an app built with Mac Catalyst.

- Start a UIContextMenuInteraction by using Force Touch or a long press gesture.

When one of these interactions happens, the system asks your view controller for content to share. Supply multiple representations of the current content, such as a file, image, and URL.

## Topics

### Providing shareable content

var activityItemsConfiguration: (any UIActivityItemsConfigurationReading)?

An object or value that specifies items to share.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- UIAccessibilityElement
- UIActionSheet
- UIActivityIndicatorView
- UIActivityViewController
- UIAlertController
- UIAlertView
- UIApplication
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
- UIProgressView
- UIReferenceLibraryViewController
- UIRefreshControl
- UIResponder
- UIScene
- UIScrollView
- UISearchBar
- UISearchContainerViewController
- UISearchController
- UISearchTextField
- UISegmentedControl
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
- UIWindowScene

## See Also

### Activities interface

Collaborating and sharing copies of your data

Share data and collaborate with people from your app.

class UIActivityViewController

A view controller that you use to offer standard services from your app.

class UIActivityItemProvider

A proxy for data that passes to an activity view controller.

protocol UIActivityItemSource

A set of methods that an activity view controller uses to retrieve the data items to act on.

class UIActivity

An abstract class that you subclass to implement app-specific services.

