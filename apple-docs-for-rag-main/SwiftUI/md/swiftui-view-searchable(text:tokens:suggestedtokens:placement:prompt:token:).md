

- SwiftUI
- View
-  searchable(text:tokens:suggestedTokens:placement:prompt:token:) 

Instance Method

# searchable(text:tokens:suggestedTokens:placement:prompt:token:)

Marks this view as searchable with text, tokens, and suggestions.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
nonisolated
func searchable(
    text: Binding,
    tokens: Binding,
    suggestedTokens: Binding,
    placement: SearchFieldPlacement = .automatic,
    prompt: S,
    @ViewBuilder token: @escaping (C.Element) -> T
) -> some View where C : MutableCollection, C : RandomAccessCollection, C : RangeReplaceableCollection, T : View, S : StringProtocol, C.Element : Identifiable
```

Show all declarations

## Parameters 

`text`  

The text to display and edit in the search field.

`tokens`  

A collection of tokens to display and edit in the search field.

`suggestedTokens`  

A collection of tokens to display as suggestions.

`placement`  

The preferred placement of the search field within the containing view hierarchy.

`prompt`  

A string representing the prompt of the search field which provides users with guidance on what to search for.

`token`  

A view builder that creates a view given an element in tokens.

## Mentioned in 

Performing a search operation

Suggesting search terms

## Discussion

For more information about using searchable modifiers, see Adding a search interface to your app.

## See Also

### Making search suggestions

Suggesting search terms

Provide suggestions to people searching for content in your app.

func searchSuggestions&lt;S>(() -> S) -> some View

Configures the search suggestions for this view.

func searchSuggestions(Visibility, for: SearchSuggestionsPlacement.Set) -> some View

Configures how to display search suggestions within this view.

func searchCompletion(_:)

Associates a fully formed string with the value of this view when used as a search suggestion.

struct SearchSuggestionsPlacement

The ways that SwiftUI displays search suggestions.

