

- AppKit
- NSTextSuggestionsDelegate
-  appending(\_:) 

Instance Method

# appending(\_:)

Returns a new text suggestions delegate of the same suggestion item type with the items and behaviors of the receiving delegate and `other` concatenated. When the returned delegate is connected to a text field, all suggestion items provided from the first suggestions delegate appear before all those from the second suggestions delegate, visually separated by a separator.

macOS 15.0+

``` source
@MainActor
func appending(_ other: some NSTextSuggestionsDelegate) -> some NSTextSuggestionsDelegate
```

Available when `SuggestionItemType` conforms to `Hashable`.

## Discussion

Note

The returned aggregate text suggestions delegate strongly retains the given text suggestions delegate (`other`).

