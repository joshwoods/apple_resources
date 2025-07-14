

- RealityKit
- ResolvedModel3D
-  searchable(text:placement:prompt:) 

Instance Method

# searchable(text:placement:prompt:)

Marks this view as searchable, which configures the display of a search field.

RealityKitSwiftUIiOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
nonisolated
func searchable(
    text: Binding,
    placement: SearchFieldPlacement = .automatic,
    prompt: Text? = nil
) -> some View
```

## Parameters 

`text`  

The text to display and edit in the search field.

`placement`  

The preferred placement of the search field within the containing view hierarchy.

`prompt`  

A `Text` view representing the prompt of the search field which provides users with guidance on what to search for.

## Discussion

For more information about using searchable modifiers, see doc:Adding-a-search-interface-to-your-app.

