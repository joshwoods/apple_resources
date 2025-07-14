

- FamilyControls
- FamilyActivityPicker
-  searchable(text:placement:prompt:) 

Instance Method

# searchable(text:placement:prompt:)

Marks this view as searchable, which configures the display of a search field.

FamilyControlsSwiftUIiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+watchOS 8.0+

``` source
nonisolated
func searchable(
    text: Binding,
    placement: SearchFieldPlacement = .automatic,
    prompt: LocalizedStringKey
) -> some View
```

## Parameters 

`text`  

The text to display and edit in the search field.

`placement`  

The preferred placement of the search field within the containing view hierarchy.

`prompt`  

The key for the localized prompt of the search field which provides users with guidance on what to search for.

## Discussion

For more information about using searchable modifiers, see doc:Adding-a-search-interface-to-your-app.

## See Also

### Search

func searchable(text: Binding&lt;String>, placement: SearchFieldPlacement, prompt: Text?) -> some View

Marks this view as searchable, which configures the display of a search field.

func searchable&lt;S>(text: Binding&lt;String>, placement: SearchFieldPlacement, prompt: S) -> some View

Marks this view as searchable, which configures the display of a search field.

func searchable&lt;S>(text: Binding&lt;String>, placement: SearchFieldPlacement, prompt: Text?, suggestions: () -> S) -> some View

Marks this view as searchable, which configures the display of a search field.

func searchable&lt;S>(text: Binding&lt;String>, placement: SearchFieldPlacement, prompt: LocalizedStringKey, suggestions: () -> S) -> some View

Marks this view as searchable, which configures the display of a search field.

func searchable&lt;V, S>(text: Binding&lt;String>, placement: SearchFieldPlacement, prompt: S, suggestions: () -> V) -> some View

Marks this view as searchable, which configures the display of a search field.

