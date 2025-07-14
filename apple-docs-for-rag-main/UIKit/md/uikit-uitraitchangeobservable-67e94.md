

- UIKit
-  UITraitChangeObservable 

Protocol

# UITraitChangeObservable

A type that calls your code in reaction to changes in the trait environment.

iOS 17.0+iPadOS 17.0+Mac CatalysttvOS 17.0+visionOS

``` source
@MainActor
protocol UITraitChangeObservable
```

## Mentioned in 

Building a desktop-class iPad app

## Overview

Types that conform to UITraitChangeObservable can execute your code in response to changes in their trait collection. When you register for trait changes, the system observes the specified traits, and calls your code when any of the observed traits change value.

Keep your trait registrations focused, and avoid doing work not directly relevant to updated traits. Traits may change more than once before the system updates a view, so avoid expensive work in response to trait changes. For example, use the trait change notification to call setNeedsDisplay(), and update your view in draw(_:).

UIKit cleans up registrations at the end of the object lifecycle. Unregister only in the rare situations when you need to dynamically change which traits you observe.

## Topics

### Observing trait changes

func registerForTraitChanges([UITrait], action: Selector) -> any UITraitChangeRegistration

Registers a list of traits to observe, and calls a method on the receiving object when one of the observed traits changes.

**Required**

func registerForTraitChanges&lt;TraitEnvironment>([UITrait], handler: Self.TraitChangeHandler&lt;TraitEnvironment>) -> any UITraitChangeRegistration

Registers a list of traits to observe and a closure to execute when one of the observed traits changes.

**Required**

func registerForTraitChanges([UITrait], target: Any, action: Selector) -> any UITraitChangeRegistration

Registers a list of traits to observe, and calls a method on the specified target object when one of the observed traits changes.

**Required**

func unregisterForTraitChanges(any UITraitChangeRegistration)

Tells the system to stop observing previously registered traits.

**Required**

typealias TraitChangeHandler

A closure the system executes when observed traits change.

protocol UITraitChangeRegistration

## Relationships

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

protocol UITraitEnvironment

A set of methods that makes the iOS interface environment available to your app.

protocol UIMutableTraits

A mutable container of traits.

protocol UIAdaptivePresentationControllerDelegate

A set of methods that, in conjunction with a presentation controller, determine how to respond to trait changes in your app.

protocol UIContentContainer

A set of methods for adapting the contents of your view controllers to size and trait changes.

