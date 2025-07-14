

- UIKit
-  UIFocusEnvironment 

Protocol

# UIFocusEnvironment

A set of methods that define the focus behavior for a branch of the view hierarchy.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
protocol UIFocusEnvironment : NSObjectProtocol
```

## Overview

The UIFocusEnvironment protocol provides a common interface for specifying and reacting to focus behavior throughout your app. Classes in UIKit that conform to this protocol include UIView, UIViewController, UIWindow, and UIPresentationController — in other words, classes that are either directly or indirectly in control of views on the screen.

## Topics

### Requesting focus update

func setNeedsFocusUpdate()

Submits a request to the focus engine for a focus update in this environment.

**Required**

func updateFocusIfNeeded()

Tells the focus engine to force a focus update immediately.

**Required**

### Validating focus movements

func shouldUpdateFocus(in: UIFocusUpdateContext) -> Bool

Returns a Boolean value indicating whether the focus engine should allow the focus update described by the specified context to occur.

**Required**

### Responding to focus updates

func didUpdateFocus(in: UIFocusUpdateContext, with: UIFocusAnimationCoordinator)

Called immediately after the system updates the focus to a new view.

**Required**

### Controlling user-generated focus movements

var preferredFocusEnvironments: [any UIFocusEnvironment]

An array of focus environments, ordered by priority, to which this environment prefers focus to be directed during a focus update.

**Required**

var preferredFocusedView: UIView?

Specifies the view that should be focused if this environment is focused.

Deprecated

### Getting the sound to play during updates

Using custom sounds for focus movement

Customize the sounds users hear when focus moves.

func soundIdentifierForFocusUpdate(in: UIFocusUpdateContext) -> UIFocusSoundIdentifier?

Asks the delegate for the identifier of the sound to play when the object gains focus.

struct UIFocusSoundIdentifier

An identifier for a focus-related sound.

### Checking the ancestry of the environment

func contains(any UIFocusEnvironment) -> Bool

Returns a Boolean value that indicates whether the focus environment contains the specified environment.

var parentFocusEnvironment: (any UIFocusEnvironment)?

The parent focus environment for this environment.

**Required**

var focusItemContainer: (any UIFocusItemContainer)?

The container for the child focus items in this focus environment.

**Required**

### Identifying the focus group

var focusGroupIdentifier: String?

The identifier of the focus group that the environment belongs to.

## Relationships

### Inherits From

- NSObjectProtocol

### Inherited By

- UIFocusItem

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

## See Also

### Focus interactions

Navigating an app’s user interface using a keyboard

Navigate between user interface elements using a keyboard and focusable UI elements in iPad apps and apps built with Mac Catalyst.

About focus interactions for Apple TV

Design and implement intuitive control schemes for menus and interactive user interface layouts.

Adding user-focusable elements to a tvOS app

Create intuitive and easily manipulated user-interactive controls for your tvOS app.

class UIFocusSystem

Queries and reevaluates the currently focused item.

class UIFocusUpdateContext

An object that provides information relevant to a specific focus update from one view to another.

protocol UIFocusItem

An object that can become focused.

class UIFocusMovementHint

Provides movement hint information for the focused item.

protocol UIFocusItemContainer

The container responsible for providing geometric context to focus items within a given focus environment.

protocol UIFocusItemScrollableContainer

A type of focus item container that supports automatic scrolling of focusable content.

struct UIFocusGroupPriority

The importance of an item within a focus group, used by the focus system to determine the group’s primary item.

