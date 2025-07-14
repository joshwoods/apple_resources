

- UIKit
-  UITraitEnvironment 

Protocol

# UITraitEnvironment

A set of methods that makes the iOS interface environment available to your app.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
protocol UITraitEnvironment : NSObjectProtocol
```

## Mentioned in 

Checking the availability of 3D Touch

## Overview

The iOS interface environment includes traits such as horizontal and vertical size class, display scale, and user interface idiom. To access the trait environment of an object that adopts this protocol, use the traitCollection property. The protocol also provides an overridable method that the system calls when the interface environment changes. Implement this method as part of creating an adaptive iOS app.

For more about trait collections, see UITraitCollection. For the WWDC 2014 presentation on creating adaptive interfaces in iOS, see Building Adaptive Apps with UIKit.

## Topics

### Accessing a trait collection

var traitCollection: UITraitCollection

The traits, such as the size class and scale factor, that describe the current environment of the object.

**Required**

### Responding to a change in the interface environment

func traitCollectionDidChange(UITraitCollection?)

Reports changes in the iOS interface environment.

**Required**

Deprecated

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
- UIPopoverPresentationController
- UIPresentationController
- UIProgressView
- UIReferenceLibraryViewController
- UIRefreshControl
- UIScreen
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
- UIWindowScene

## See Also

### Adaptivity

Automatic trait tracking

Reduce the need to manually register for trait changes when you use traits within a method or closure that supports automatic trait tracking.

Responding to changing display modes on Apple TV

Change images and resources dynamically when the screen gamut on your device changes.

class UITraitCollection

A collection of data that represents the environment for an individual element in your app’s user interface.

protocol UITraitChangeObservable

A type that calls your code in reaction to changes in the trait environment.

protocol UIMutableTraits

A mutable container of traits.

protocol UIAdaptivePresentationControllerDelegate

A set of methods that, in conjunction with a presentation controller, determine how to respond to trait changes in your app.

protocol UIContentContainer

A set of methods for adapting the contents of your view controllers to size and trait changes.

