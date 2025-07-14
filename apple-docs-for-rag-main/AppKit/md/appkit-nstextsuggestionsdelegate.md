

- AppKit
-  NSTextSuggestionsDelegate 

Protocol

# NSTextSuggestionsDelegate

A protocol for suggestion delegates of text fields to conform to in order to provide text suggestions in response to the user typing.

macOS 15.0+

``` source
@MainActor
protocol NSTextSuggestionsDelegate : AnyObject
```

## Topics

### Associated Types

associatedtype SuggestionItemType

The type of the `representedValue` property of the provided suggestion items (`NSSuggestionItem`).

**Required**

### Instance Methods

func appending(some NSTextSuggestionsDelegate&lt;Self.SuggestionItemType>) -> some NSTextSuggestionsDelegate&lt;Self.SuggestionItemType> 

Returns a new text suggestions delegate of the same suggestion item type with the items and behaviors of the receiving delegate and `other` concatenated. When the returned delegate is connected to a text field, all suggestion items provided from the first suggestions delegate appear before all those from the second suggestions delegate, visually separated by a separator.

func appending&lt;T>(some NSTextSuggestionsDelegate) -> some NSTextSuggestionsDelegate&lt;AnyHashable> 

Returns a new text suggestions delegate of a different, but `Hashable` suggestion item type with the items and behaviors of the receiving delegate and `other` concatenated. When the returned delegate is connected to a text field, all suggestion items provided from the first suggestions delegate appear before all those from the second suggestions delegate, visually separated by a separator.

func textField(NSTextField, didSelect: Self.Item)

Called when an item in the suggestions menu has been selected.

**Required** Default implementation provided.

func textField(NSTextField, provideUpdatedSuggestions: (Self.ItemResponse) -> Void)

Called when the text field’s text (or tokens) have changed and when the text field is going to display a new list of suggestion items.

**Required**

func textField(NSTextField, textCompletionFor: Self.Item) -> String?

Returns the full completion text for a particular item to use when the item is highlighted or selected.

**Required** Default implementation provided.

### Type Aliases

typealias Item

A suggestion item with the same suggestion item type as the delegate.

typealias ItemResponse

A suggestion item response with the same generic type as the delegate.

typealias ItemSection

A suggestion item section with the same suggestion item type as the controller.

