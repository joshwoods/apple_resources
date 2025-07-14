

- UIKit
-  UIPasteConfigurationSupporting 

Protocol

# UIPasteConfigurationSupporting

The interface that determines whether a responder object supports paste configuration.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
protocol UIPasteConfigurationSupporting : NSObjectProtocol
```

## Topics

### Accessing the paste configuration

var pasteConfiguration: UIPasteConfiguration?

The paste configuration associated with the responder object.

**Required**

### Performing a paste operation

func canPaste([NSItemProvider]) -> Bool

Returns a Boolean value that determines whether the responder object can perform a paste operation using data provided by the item providers.

func paste(itemProviders: [NSItemProvider])

Performs a paste operation on the responder object.

## Relationships

### Inherits From

- NSObjectProtocol

### Inherited By

- UITextDroppable
- UITextPasteConfigurationSupporting

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

### Pasteboard

class UIPasteControl

A button that a person taps to place pasteboard contents in your app.

class Configuration

An object that determines a paste button’s color, corner style, icon, and text.

enum DisplayMode

Options that determine whether a paste button composes an icon, textual label, or both.

class UIPasteboard

An object that helps a user share data from one place to another within your app, and from your app to other apps.

class UIPasteConfiguration

The interface that an object implements to declare its ability to accept specific data types for pasting and for drag-and-drop activities.

