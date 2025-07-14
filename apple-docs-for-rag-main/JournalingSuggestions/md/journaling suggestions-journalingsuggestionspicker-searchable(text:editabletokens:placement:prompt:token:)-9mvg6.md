

- Journaling Suggestions
- JournalingSuggestionsPicker
-  searchable(text:editableTokens:placement:prompt:token:) 

Instance Method

# searchable(text:editableTokens:placement:prompt:token:)

Marks this view as searchable, which configures the display of a search field.

Journaling SuggestionsSwiftUIiOS 17.0+macOS 14.0+

``` source
nonisolated
func searchable(
    text: Binding,
    editableTokens: Binding,
    placement: SearchFieldPlacement = .automatic,
    prompt: Text? = nil,
    @ViewBuilder token: @escaping (Binding) -> some View
) -> some View where C : RandomAccessCollection, C : RangeReplaceableCollection, C.Element : Identifiable
```

## Parameters 

`text`  

The text to display and edit in the search field.

`editableTokens`  

A collection of tokens to display and edit in the search field.

`placement`  

The preferred placement of the search field within the containing view hierarchy.

`prompt`  

A `Text` view representing the prompt of the search field which provides users with guidance on what to search for.

`token`  

A view builder that creates a view given an element in tokens.

## Discussion

For more information about using searchable modifiers, see doc:Adding-a-search-interface-to-your-app.

