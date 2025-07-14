

- Assignables
- AssignableDocumentView
-  searchable(text:placement:prompt:suggestions:) 

Instance Method

# searchable(text:placement:prompt:suggestions:)

Marks this view as searchable, which configures the display of a search field.

AssignablesSwiftUIiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
nonisolated
func searchable(
    text: Binding,
    placement: SearchFieldPlacement = .automatic,
    prompt: Text? = nil,
    @ViewBuilder suggestions: () -> S
) -> some View where S : View
```

## Parameters 

`text`  

The text to display and edit in the search field.

`placement`  

Where the search field should attempt to be placed based on the containing view hierarchy.

`prompt`  

A `Text` view representing the prompt of the search field which provides users with guidance on what to search for.

`suggestions`  

A view builder that produces content that populates a list of suggestions.

## Discussion

For more information about using searchable modifiers, see doc:Adding-a-search-interface-to-your-app.

