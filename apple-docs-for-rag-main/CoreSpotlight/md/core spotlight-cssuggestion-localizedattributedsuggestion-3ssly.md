

- Core Spotlight
- CSSuggestion
-  localizedAttributedSuggestion 

Instance Property

# localizedAttributedSuggestion

An attributed string for the localized suggestion.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
var localizedAttributedSuggestion: AttributedString { get }
```

## Discussion

The `localizedAttributedString` provides the suggestion text that the system uses to replace the text in the search bar. The system uses the attributed string to highlight the range of the suggestion string that matches the user query string.

For example, the user types “search”, and the system offers a suggestion for “search suggestion”, where the system marks up “search” using the CSSuggestionHighlightAttributeName. Your app can use the range to add a bold highlight, if desired.

## See Also

### Setting suggestion attributes

var suggestionKind: CSSuggestion.SuggestionKind

The type of suggestion.

enum SuggestionKind

The suggestion type that determines how the system handles a suggestion.

