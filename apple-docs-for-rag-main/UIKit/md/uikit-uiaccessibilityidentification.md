

- UIKit
-  UIAccessibilityIdentification 

Protocol

# UIAccessibilityIdentification

Methods that associate a unique identifier with elements in your user interface.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
protocol UIAccessibilityIdentification : NSObjectProtocol
```

## Overview

You can use the identifiers you define in UI Automation scripts because the value of accessibilityIdentifier corresponds to the return value of the name method of `UIAElement`.

## Topics

### Accessing an element identifier

var accessibilityIdentifier: String?

A string that identifies the element.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- UIAccessibilityElement
- UIAction
- UIActionSheet
- UIActivityIndicatorView
- UIAlertAction
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
- UICommand
- UIContentUnavailableView
- UIControl
- UIDatePicker
- UIDeferredMenuElement
- UIEventAttributionView
- UIImage
- UIImageView
- UIInputView
- UIKeyCommand
- UILabel
- UIListContentView
- UIMenu
- UIMenuElement
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
- UIView
- UIVisualEffectView
- UIWebView
- UIWindow
- UIWindowScene.ActivationAction

## See Also

### Behaviors

UIAccessibilityFocus

An informal protocol that provides a way to determine whether an assistive app, such as VoiceOver, has focus on an accessible element.

protocol UIAccessibilityReadingContent

Methods to implement for an object that represents content that users read, such as a book or an article.

protocol UIAccessibilityContentSizeCategoryImageAdjusting

Methods to determine when to adjust images for different content size categories.

struct UIAccessibilityTextualContext

Constants that describe a named context that helps identify and classify the type of text inside an element.

