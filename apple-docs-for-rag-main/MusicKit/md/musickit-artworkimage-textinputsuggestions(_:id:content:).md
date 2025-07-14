

- MusicKit
- ArtworkImage
-  textInputSuggestions(\_:id:content:) 

Instance Method

# textInputSuggestions(\_:id:content:)

Configures the text input suggestions for this view.

MusicKitSwiftUImacOS 15.0+

``` source
nonisolated
func textInputSuggestions(
    _ data: Data,
    id: KeyPath,
    @ViewBuilder content: @escaping (Data.Element) -> Content
) -> some View where Data : RandomAccessCollection, ID : Hashable, Content : View
```

## Parameters 

`data`  

The data that is used to create views dynamically.

`id`  

The key path to the provided data’s identifier.

`content`  

The view builder that creates views dynamically.

## Discussion

You can suggest text completions during a text input operation by providing data to this modifier. The interface presents the suggestion views as a list of choices when someone activates the text editing interface.

Associate a string with each suggestion view by adding the `View/textInputCompletion(_:)` modifier to the view.

Use `Label` to get platform-standard visual representations of suggestion text accompanied with images, and `Section` for labelled sections of results.

