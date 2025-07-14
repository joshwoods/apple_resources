

- Journaling Suggestions
- JournalingSuggestionsPicker
-  onDrag(\_:) 

Instance Method

# onDrag(\_:)

Activates this view as the source of a drag and drop operation.

Journaling SuggestionsSwiftUIiOS 13.4+macOS 10.15+

``` source
nonisolated
func onDrag(_ data: @escaping () -> NSItemProvider) -> some View
```

## Parameters 

`data`  

A closure that returns a single NSItemProvider that represents the draggable data from this view.

## Return Value

A view that activates this view as the source of a drag and drop operation, beginning with user gesture input.

## Discussion

Applying the `onDrag(_:)` modifier adds the appropriate gestures for drag and drop to this view. When a drag operation begins, a rendering of this view is generated and used as the preview image.

To customize the default preview, apply a `View/contentShape(_:_:eoFill:)` with a `ContentShapeKinds/dragPreview` kind. For example, you can change the preview’s corner radius or use a nested view as the preview.

If you want to show a different preview, you can use `View/onDrag(_:preview:)`.

