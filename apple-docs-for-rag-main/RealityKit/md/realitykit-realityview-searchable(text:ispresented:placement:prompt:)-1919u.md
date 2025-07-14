

- RealityKit
- RealityView
-  searchable(text:isPresented:placement:prompt:) 

Instance Method

# searchable(text:isPresented:placement:prompt:)

Marks this view as searchable with programmatic presentation of the search field.

RealityKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+visionOS

``` source
nonisolated
func searchable(
    text: Binding,
    isPresented: Binding,
    placement: SearchFieldPlacement = .automatic,
    prompt: Text? = nil
) -> some View
```

## Parameters 

`text`  

The text to display and edit in the search field.

`isPresenting`  

A `Binding` that controls the presented state of search.

`placement`  

The preferred placement of the search field within the containing view hierarchy.

`prompt`  

A `Text` view representing the prompt of the search field which provides users with guidance on what to search for.

## Discussion

For more information about using searchable modifiers, see doc:Adding-a-search-interface-to-your-app. For information about presenting a search field programmatically, see doc:Managing-search-interface-activation.

