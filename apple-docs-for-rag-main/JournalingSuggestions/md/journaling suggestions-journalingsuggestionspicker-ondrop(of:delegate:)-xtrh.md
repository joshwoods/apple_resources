

- Journaling Suggestions
- JournalingSuggestionsPicker
-  onDrop(of:delegate:) 

Instance Method

# onDrop(of:delegate:)

Defines the destination for a drag and drop operation with the same size and position as this view, with behavior controlled by the given delegate.

Journaling SuggestionsSwiftUIiOS 13.4–18.4DeprecatedmacOS 10.15+visionOS 1.0+

``` source
nonisolated
func onDrop(
    of supportedTypes: [String],
    delegate: any DropDelegate
) -> some View
```

## Parameters 

`supportedTypes`  

The uniform type identifiers that describe the types of content this view can accept through drag and drop. If the drag and drop operation doesn’t contain any of the supported types, then this drop destination doesn’t activate and `isTargeted` doesn’t update.

`delegate`  

A type that conforms to the `DropDelegate` protocol. You have comprehensive control over drop behavior when you use a delegate.

## Return Value

A view that provides a drop destination for a drag operation of the specified types.

