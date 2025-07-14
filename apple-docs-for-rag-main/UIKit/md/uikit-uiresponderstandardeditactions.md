

- UIKit
-  UIResponderStandardEditActions 

Protocol

# UIResponderStandardEditActions

A set of standard methods that apps can adopt to support editing.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
protocol UIResponderStandardEditActions : NSObjectProtocol
```

## Overview

Responder objects can implement the methods of this protocol to handle standard editing-related actions. For example, a UIEditMenuInteraction object displays the actions in an edit menu using these methods. UIKit searches the responder chain for an object that implements the appropriate method, calling the method on the first object that implements it.

## Topics

### Handling copy, cut, paste, and delete commands

func cut(Any?)

Removes the selected content and writes the data for it to the pasteboard.

func copy(Any?)

Copies the selected content to the pasteboard.

func paste(Any?)

Pastes the current contents of the pasteboard into your app’s interface.

func pasteAndGo(Any?)

Pastes the current contents of the pasteboard into your app’s interface and navigates to the entity it references.

func pasteAndMatchStyle(Any?)

Pastes the current contents of the pasteboard into your app’s interface using the text style of the target.

func pasteAndSearch(Any?)

Pastes the current contents of the pasteboard into your app’s interface and performs a search.

func delete(Any?)

Removes the selected content from your interface.

### Handling find and replace commands

func find(Any?)

Begins a search for content in your app’s interface.

func findNext(Any?)

Finds the next match in your app’s interface.

func findPrevious(Any?)

Finds the previous match in your app’s interface.

func findAndReplace(Any?)

Begins a search for content in your app’s interface and provides a replacement.

func useSelectionForFind(Any?)

Begins a search for the selected content in your app’s interface.

### Handling selection commands

func select(Any?)

Selects the content in your responder.

func selectAll(Any?)

Selects all of the content in the current responder.

### Handling data commands

func duplicate(Any?)

Duplicates data.

func export(Any?)

Exports data in different file formats or to other apps.

func move(Any?)

Prompts a person to specify a new location and moves data to that location.

func rename(Any?)

Changes a title.

### Handling a print command

func printContent(Any?)

Tells your app to print available content.

### Handling styled text editing

func toggleBoldface(Any?)

Toggles the bold style information of the selected text.

func toggleItalics(Any?)

Toggles the italic style information of the selected text.

func toggleUnderline(Any?)

Toggles the underline style information of the selected text.

### Handling writing direction changes

func makeTextWritingDirectionLeftToRight(Any?)

Changes the writing direction to left-to-right.

func makeTextWritingDirectionRightToLeft(Any?)

Changes the writing direction to right-to-left.

### Handling size changes

func increaseSize(Any?)

Increases the size of the current object by one unit.

func decreaseSize(Any?)

Decreases the size of the current object by one unit.

### Handling other text formatting changes

func updateTextAttributes(conversionHandler: ([NSAttributedString.Key : Any]) -> [NSAttributedString.Key : Any])

Tells your app to update the attributes of the currently selected text.

### Instance Methods

func showWritingTools(Any)

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

### Edit menus

class UIEditMenuInteraction

An interaction that provides edit operations using a menu.

protocol UIEditMenuInteractionDelegate

The methods for customizing the menu the interaction displays.

class UIEditMenuConfiguration

An object containing the configuration details for the menu your app presents in response to an edit menu interaction.

