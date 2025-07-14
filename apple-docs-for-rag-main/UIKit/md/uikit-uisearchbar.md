

- UIKit
-  UISearchBar 

Class

# UISearchBar

A specialized view for receiving search-related information from the user.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class UISearchBar
```

## Overview

UISearchBar provides a text field for entering text, a search button, a bookmark button, and a cancel button. A search bar doesn’t actually perform any searches. You use a delegate, an object conforming to the UISearchBarDelegate protocol, to implement the actions when the user enters text or clicks buttons. For details about interacting with the text field, accessing its content, and using tokens, see UISearchTextField and UISearchToken.

### Customize appearance

You can customize the appearance of search bars one at a time, or you can use the appearance proxy (`[UISearchBar appearance]`) to customize the appearance of all search bars in an app.

In general, you should specify a value for the normal state to be used by other states which don’t have a custom value set. Similarly, when a property is dependent on the bar metrics (on iPhone, in landscape orientation bars have a different height from standard), you should specify a value for `UIBarMetricsDefault`.

## Topics

### Creating a search bar

convenience init()

Initializes the search bar to its default state.

init?(coder: NSCoder)

Creates a search bar from data in a given unarchiver.

init(frame: CGRect)

Creates a search bar with a specified frame.

### Handling search bar interactions

var delegate: (any UISearchBarDelegate)?

The search bar’s delegate object.

protocol UISearchBarDelegate

A collection of optional methods that you implement to make a search bar control functional.

### Getting the search text

var placeholder: String?

The string to display when there’s no other text in the text field.

var prompt: String?

A single line of text displayed at the top of the search bar.

var text: String?

The current or starting search text.

var searchTextField: UISearchTextField

The text field that the user enters a search query into.

### Configuring the search bar

var isEnabled: Bool

A Boolean value indicating whether the search bar is in the enabled state.

var barTintColor: UIColor?

The tint color to apply to the search bar background.

var searchBarStyle: UISearchBar.Style

A search bar style that specifies the search bar’s appearance.

enum Style

Specifies whether the search bar has a background.

var tintColor: UIColor!

The tint color to apply to key elements in the search bar.

var isTranslucent: Bool

A Boolean value that indicates whether the search bar is translucent (true) or not (false).

var barStyle: UIBarStyle

A bar style that specifies the search bar’s appearance.

enum UIBarStyle

Defines the stylistic appearance of different types of views.

### Customizing the keyboard shortcut items

var inputAssistantItem: UITextInputAssistantItem

The input assistant to use for configuring the keyboard’s shortcuts bar.

### Configuring the search interface

var showsBookmarkButton: Bool

A Boolean value indicating whether the bookmark button is displayed.

var showsCancelButton: Bool

A Boolean value indicating whether the cancel button is displayed.

func setShowsCancelButton(Bool, animated: Bool)

Sets the display state of the cancel button optionally with animation.

var showsSearchResultsButton: Bool

A Boolean value indicating whether the search results button is displayed.

var isSearchResultsButtonSelected: Bool

A Boolean value indicating whether the search results button is selected.

### Customizing the search bar appearance

var backgroundImage: UIImage?

The background image for the search bar.

func backgroundImage(for: UIBarPosition, barMetrics: UIBarMetrics) -> UIImage?

Returns the image used for the background in a given position and with given metrics.

func setBackgroundImage(UIImage?, for: UIBarPosition, barMetrics: UIBarMetrics)

Sets the image to use for the background in a given position and with given metrics.

func image(for: UISearchBar.Icon, state: UIControl.State) -> UIImage?

Returns the image for a given search bar icon type and control state.

func setImage(UIImage?, for: UISearchBar.Icon, state: UIControl.State)

Sets the image for a given search bar icon type and control state.

func positionAdjustment(for: UISearchBar.Icon) -> UIOffset

Returns the position adjustment for a given icon.

func setPositionAdjustment(UIOffset, for: UISearchBar.Icon)

Returns the position adjustment for a given icon.

var inputAccessoryView: UIView?

A custom input accessory view for the keyboard of the search bar.

func searchFieldBackgroundImage(for: UIControl.State) -> UIImage?

Returns the search text field image for a given state.

func setSearchFieldBackgroundImage(UIImage?, for: UIControl.State)

Sets the search text field image for a given state.

var searchFieldBackgroundPositionAdjustment: UIOffset

The offset of the search text field background in the search bar.

var searchTextPositionAdjustment: UIOffset

The offset of the text within the search text field background.

### Configuring scope bar buttons

var scopeButtonTitles: [String]?

An array of strings indicating the titles of the scope buttons.

var selectedScopeButtonIndex: Int

The index of the selected scope button.

var showsScopeBar: Bool

Specifies whether the scope bar is displayed.

func setShowsScope(Bool, animated: Bool)

Specifies whether the scope bar is displayed, optionally using an animation.

### Customizing the scope bar appearance

var scopeBarBackgroundImage: UIImage?

The background image for the scope bar.

func scopeBarButtonBackgroundImage(for: UIControl.State) -> UIImage?

Returns the background image for the scope bar button in a given state.

func setScopeBarButtonBackgroundImage(UIImage?, for: UIControl.State)

Sets the background image for the scope bar button in a given state.

func scopeBarButtonDividerImage(forLeftSegmentState: UIControl.State, rightSegmentState: UIControl.State) -> UIImage?

Returns the divider image to use for a given combination of left and right segment states.

func setScopeBarButtonDividerImage(UIImage?, forLeftSegmentState: UIControl.State, rightSegmentState: UIControl.State)

Sets the divider image to use for a given combination of left and right segment states.

func scopeBarButtonTitleTextAttributes(for: UIControl.State) -> [NSAttributedString.Key : Any]?

Returns the text attributes for the search bar’s button’s title string for a given state.

func setScopeBarButtonTitleTextAttributes([NSAttributedString.Key : Any]?, for: UIControl.State)

Sets the text attributes for the search bar’ button’s title string for a given state.

### Managing dictation

var isLookToDictateEnabled: Bool

protocol UILookToDictateCapable

### Constants

enum Icon

Constants to identify the icons used in the search bar.

## Relationships

### Inherits From

- UIView

### Conforms To

- CALayerDelegate
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSTouchBarProvider
- Sendable
- UIAccessibilityIdentification
- UIActivityItemsConfigurationProviding
- UIAppearance
- UIAppearanceContainer
- UIBarPositioning
- UICoordinateSpace
- UIDynamicItem
- UIFocusEnvironment
- UIFocusItem
- UIFocusItemContainer
- UILargeContentViewerItem
- UILookToDictateCapable
- UIPasteConfigurationSupporting
- UIPopoverPresentationControllerSourceItem
- UIResponderStandardEditActions
- UITextInputTraits
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Search interface

class UISearchContainerViewController

A view controller that manages the presentation of search results in your interface.

class UISearchController

A view controller that manages the display of search results based on interactions with a search bar.

protocol UISearchResultsUpdating

A set of methods that let you update search results based on information the user enters into the search bar.

Displaying searchable content by using a search controller

Create a user interface with searchable content in a table view.

Using suggested searches with a search controller

Create a search interface with a table view of suggested searches.

