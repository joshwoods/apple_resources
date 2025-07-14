

- SwiftUI
- View
-  searchable(text:editableTokens:isPresented:placement:prompt:token:) 

Instance Method

# searchable(text:editableTokens:isPresented:placement:prompt:token:)

Marks this view as searchable, which configures the display of a search field.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
nonisolated
func searchable(
    text: Binding,
    editableTokens: Binding,
    isPresented: Binding,
    placement: SearchFieldPlacement = .automatic,
    prompt: LocalizedStringKey,
    @ViewBuilder token: @escaping (Binding) -> some View
) -> some View where C : RandomAccessCollection, C : RangeReplaceableCollection, C.Element : Identifiable
```

Show all declarations

## Parameters 

`text`  

The text to display and edit in the search field.

`editableTokens`  

A collection of tokens to display and edit in the search field.

`placement`  

The preferred placement of the search field within the containing view hierarchy.

`prompt`  

The key for the localized prompt of the search field which provides users with guidance on what to search for.

`token`  

A view builder that creates a view given an element in tokens.

## Discussion

For more information about using searchable modifiers, see Adding a search interface to your app.

## See Also

### Detecting, activating, and dismissing search

Managing search interface activation

Programmatically detect and dismiss a search field.

var isSearching: Bool

A Boolean value that indicates when the user is searching.

var dismissSearch: DismissSearchAction

An action that ends the current search interaction.

struct DismissSearchAction

An action that can end a search interaction.

func searchable(text:isPresented:placement:prompt:)

Marks this view as searchable with programmatic presentation of the search field.

func searchable(text:tokens:isPresented:placement:prompt:token:)

Marks this view as searchable with text and tokens, as well as programmatic presentation.

func searchable(text:tokens:suggestedTokens:isPresented:placement:prompt:token:)

Marks this view as searchable with text, tokens, and suggestions, as well as programmatic presentation.

