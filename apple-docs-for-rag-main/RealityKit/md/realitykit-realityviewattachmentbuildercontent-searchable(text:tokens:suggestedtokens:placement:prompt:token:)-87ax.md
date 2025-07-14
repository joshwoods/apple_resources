

- RealityKit
- RealityViewAttachmentBuilderContent
-  searchable(text:tokens:suggestedTokens:placement:prompt:token:) 

Instance Method

# searchable(text:tokens:suggestedTokens:placement:prompt:token:)

Marks this view as searchable with text, tokens, and suggestions.

RealityKitSwiftUIiOS 16.0+iPadOS 16.0+macOS 13.0+visionOS

``` source
nonisolated
func searchable(
    text: Binding,
    tokens: Binding,
    suggestedTokens: Binding,
    placement: SearchFieldPlacement = .automatic,
    prompt: Text? = nil,
    @ViewBuilder token: @escaping (C.Element) -> T
) -> some View where C : MutableCollection, C : RandomAccessCollection, C : RangeReplaceableCollection, T : View, C.Element : Identifiable
```

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

A `Text` view representing the prompt of the search field which provides users with guidance on what to search for.

`token`  

A view builder that creates a view given an element in tokens.

## Discussion

For more information about using searchable modifiers, see doc:Adding-a-search-interface-to-your-app.

