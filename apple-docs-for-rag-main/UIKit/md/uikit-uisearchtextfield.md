

- UIKit
-  UISearchTextField 

Class

# UISearchTextField

A view for displaying and editing text and search tokens.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class UISearchTextField
```

## Overview

Use a search text field to display search criteria represented as text and tokens, and allow the user to edit that criteria. Tokens are discrete representations of nontextual content that your app can create and use to represent filters that limit the search results. Tokens always occur contiguously before any text in the search field.

UISearchBar hosts a search text field, but you may also use a search text field in other roles, such as the title view of a UINavigationItem.

Note

The search field assigns text positions (UITextPosition) to tokens as well as text so that users can interact with tokens using selection gestures and keyboard input. If the current selection includes any tokens, selectedTextRange includes their positions. Use the search field’s textualRange property to access the range of just the text without the tokens.

Tokens can be programmatically selected by including their position in a range assigned to the selectedTextRange property.

## Topics

### Converting text into tokens

func replaceTextualPortion(of: UITextRange, with: UISearchToken, at: Int)

Converts text in a search field into a search token.

var textualRange: UITextRange

The range of the field’s text content.

### Supporting token interactions

var allowsDeletingTokens: Bool

A Boolean that indicates whether the user can remove tokens from the search field.

var allowsCopyingTokens: Bool

A Boolean that indicates whether the user can copy or drag tokens from the search field.

var delegate: (any UITextFieldDelegate)?

The text field’s delegate.

protocol UISearchTextFieldDelegate

The interface for the delegate of a search field.

protocol UISearchTextFieldPasteItem

A protocol that supports pasting tokens.

### Adding and removing tokens

var tokens: [UISearchToken]

The collection of tokens in the search text field.

func insertToken(UISearchToken, at: Int)

Adds a search token at a specific index.

func removeToken(at: Int)

Removes a particular search token from the search text field.

### Customizing token behavior

var tokenBackgroundColor: UIColor!

The background color for all tokens in the search text field.

func tokens(in: UITextRange) -> [UISearchToken]

Returns the search field’s tokens that are within a given range.

func positionOfToken(at: Int) -> UITextPosition

Converts a token index into a text position.

### Providing search suggestions

var searchSuggestions: [any UISearchSuggestion]?

A list of suggestions to offer as shortcuts below the search field.

## Relationships

### Inherits From

- UITextField

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
- UIContentSizeCategoryAdjusting
- UIContextMenuInteractionDelegate
- UICoordinateSpace
- UIDynamicItem
- UIFocusEnvironment
- UIFocusItem
- UIFocusItemContainer
- UIKeyInput
- UILargeContentViewerItem
- UILetterformAwareAdjusting
- UIPasteConfigurationSupporting
- UIPopoverPresentationControllerSourceItem
- UIResponderStandardEditActions
- UITextDraggable
- UITextDroppable
- UITextInput
- UITextInputTraits
- UITextPasteConfigurationSupporting
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Search field

class UISearchToken

Search criteria in a search text field, represented by text and an optional icon.

protocol UISearchTextFieldDelegate

The interface for the delegate of a search field.

