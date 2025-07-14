

- FamilyControls
- FamilyActivityPicker
-  searchable(text:tokens:suggestedTokens:isPresented:placement:prompt:token:) 

Instance Method

# searchable(text:tokens:suggestedTokens:isPresented:placement:prompt:token:)

Marks this view as searchable with text, tokens, and suggestions, as well as programmatic presentation.

FamilyControlsSwiftUIiOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+

``` source
nonisolated
func searchable(
    text: Binding,
    tokens: Binding,
    suggestedTokens: Binding,
    isPresented: Binding,
    placement: SearchFieldPlacement = .automatic,
    prompt: S,
    @ViewBuilder token: @escaping (C.Element) -> T
) -> some View where C : MutableCollection, C : RandomAccessCollection, C : RangeReplaceableCollection, T : View, S : StringProtocol, C.Element : Identifiable
```

## Parameters 

`text`  

The text to display and edit in the search field.

`tokens`  

A collection of tokens to display and edit in the search field.

`suggestedTokens`  

A collection of tokens to display as suggestions.

`isPresenting`  

A `Binding` that controls the presented state of search.

`placement`  

The preferred placement of the search field within the containing view hierarchy.

`prompt`  

A string representing the prompt of the search field which provides users with guidance on what to search for.

`token`  

A view builder that creates a view given an element in tokens.

## Discussion

For more information about using searchable modifiers, see doc:Adding-a-search-interface-to-your-app. For information about presenting a search field programmatically, see doc:Managing-search-interface-activation.

