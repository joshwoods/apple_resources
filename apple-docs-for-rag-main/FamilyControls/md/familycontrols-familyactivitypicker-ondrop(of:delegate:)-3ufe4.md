

- FamilyControls
- FamilyActivityPicker
-  onDrop(of:delegate:) 

Instance Method

# onDrop(of:delegate:)

Defines the destination of a drag and drop operation using behavior controlled by the delegate that you provide.

FamilyControlsSwiftUIiOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+

``` source
nonisolated
func onDrop(
    of supportedContentTypes: [UTType],
    delegate: any DropDelegate
) -> some View
```

## Parameters 

`supportedContentTypes`  

The uniform type identifiers that describe the types of content this view can accept through drag and drop. If the drag and drop operation doesn’t contain any of the supported types, then this drop destination doesn’t activate and `isTargeted` doesn’t update.

`delegate`  

A type that conforms to the `DropDelegate` protocol. You have comprehensive control over drop behavior when you use a delegate.

## Return Value

A view that provides a drop destination for a drag operation of the specified types.

## Discussion

The drop destination is the same size and position as this view.

## See Also

### Drag and Drop

func onDrag&lt;V>(() -> NSItemProvider, preview: () -> V) -> some View

Activates this view as the source of a drag and drop operation.

func onDrag(() -> NSItemProvider) -> some View

Activates this view as the source of a drag and drop operation.

func itemProvider(Optional&lt;() -> NSItemProvider?>) -> some View

Provides a closure that vends the drag representation to be used for a particular data element.

func onDrop(of: [UTType], isTargeted: Binding&lt;Bool>?, perform: ([NSItemProvider]) -> Bool) -> some View

Defines the destination of a drag-and-drop operation that handles the dropped content with a closure that you specify.

func onDrop(of: [UTType], isTargeted: Binding&lt;Bool>?, perform: ([NSItemProvider], CGPoint) -> Bool) -> some View

Defines the destination of a drag and drop operation that handles the dropped content with a closure that you specify.

