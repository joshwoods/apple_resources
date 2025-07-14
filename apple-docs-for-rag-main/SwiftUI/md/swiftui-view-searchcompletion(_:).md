

- SwiftUI
- View
-  searchCompletion(\_:) 

Instance Method

# searchCompletion(\_:)

Associates a fully formed string with the value of this view when used as a search suggestion.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
nonisolated
func searchCompletion(_ completion: String) -> some View
```

Show all declarations

## Mentioned in 

Suggesting search terms

## Discussion

Use this method to associate a fully formed string with a view that is within a search suggestion list context. The system uses this value when the view is selected to replace the partial text being currently edited of the associated search field.

On tvOS, the string that you provide to the this modifier is used when displaying the associated suggestion and when replacing the partial text of the search field.

```
SearchPlaceholderView()
    .searchable(text: $text) {
        Text("🍎").searchCompletion("apple")
        Text("🍐").searchCompletion("pear")
        Text("🍌").searchCompletion("banana")
    }
```

## See Also

### Making search suggestions

Suggesting search terms

Provide suggestions to people searching for content in your app.

func searchSuggestions&lt;S>(() -> S) -> some View

Configures the search suggestions for this view.

func searchSuggestions(Visibility, for: SearchSuggestionsPlacement.Set) -> some View

Configures how to display search suggestions within this view.

func searchable(text:tokens:suggestedTokens:placement:prompt:token:)

Marks this view as searchable with text, tokens, and suggestions.

struct SearchSuggestionsPlacement

The ways that SwiftUI displays search suggestions.

