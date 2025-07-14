

- FamilyControls
- FamilyActivityPicker
-  onDrag(\_:) 

Instance Method

# onDrag(\_:)

Activates this view as the source of a drag and drop operation.

FamilyControlsSwiftUIiOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+macOS 10.15+

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

## See Also

### Drag and Drop

func onDrag&lt;V>(() -> NSItemProvider, preview: () -> V) -> some View

Activates this view as the source of a drag and drop operation.

func itemProvider(Optional&lt;() -> NSItemProvider?>) -> some View

Provides a closure that vends the drag representation to be used for a particular data element.

func onDrop(of: [UTType], delegate: any DropDelegate) -> some View

Defines the destination of a drag and drop operation using behavior controlled by the delegate that you provide.

func onDrop(of: [UTType], isTargeted: Binding&lt;Bool>?, perform: ([NSItemProvider]) -> Bool) -> some View

Defines the destination of a drag-and-drop operation that handles the dropped content with a closure that you specify.

func onDrop(of: [UTType], isTargeted: Binding&lt;Bool>?, perform: ([NSItemProvider], CGPoint) -> Bool) -> some View

Defines the destination of a drag and drop operation that handles the dropped content with a closure that you specify.

