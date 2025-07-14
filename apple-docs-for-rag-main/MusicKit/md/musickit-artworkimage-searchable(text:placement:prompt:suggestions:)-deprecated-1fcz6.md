

- MusicKit
- ArtworkImage
-  searchable(text:placement:prompt:suggestions:) Deprecated

Instance Method

# searchable(text:placement:prompt:suggestions:)

Marks this view as searchable, which configures the display of a search field.

MusicKitSwiftUIiOS 15.0–18.4DeprecatediPadOS 15.0–18.4DeprecatedMac Catalyst 15.0–18.4DeprecatedmacOS 12.0–15.4DeprecatedtvOS 15.0–18.4DeprecatedvisionOS 1.0+watchOS 8.0–11.4Deprecated

``` source
nonisolated
func searchable(
    text: Binding,
    placement: SearchFieldPlacement = .automatic,
    prompt: LocalizedStringKey,
    @ViewBuilder suggestions: () -> S
) -> some View where S : View
```

Deprecated

Use the searchable modifier with the searchSuggestions modifier

## Parameters 

`text`  

The text to display and edit in the search field.

`placement`  

Where the search field should attempt to be placed based on the containing view hierarchy.

`prompt`  

A key for the localized prompt of the search field which provides users with guidance on what to search for.

`suggestions`  

A view builder that produces content that populates a list of suggestions.

## Discussion

For more information about using searchable modifiers, see doc:Adding-a-search-interface-to-your-app.

