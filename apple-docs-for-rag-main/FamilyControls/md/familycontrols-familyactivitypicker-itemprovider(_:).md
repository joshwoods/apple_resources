

- FamilyControls
- FamilyActivityPicker
-  itemProvider(\_:) 

Instance Method

# itemProvider(\_:)

Provides a closure that vends the drag representation to be used for a particular data element.

FamilyControlsSwiftUIiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+watchOS 6.0+

``` source
nonisolated
func itemProvider(_ action: Optional NSItemProvider?>) -> some View
```

## See Also

### Drag and Drop

func onDrag&lt;V>(() -> NSItemProvider, preview: () -> V) -> some View

Activates this view as the source of a drag and drop operation.

func onDrag(() -> NSItemProvider) -> some View

Activates this view as the source of a drag and drop operation.

func onDrop(of: [UTType], delegate: any DropDelegate) -> some View

Defines the destination of a drag and drop operation using behavior controlled by the delegate that you provide.

func onDrop(of: [UTType], isTargeted: Binding&lt;Bool>?, perform: ([NSItemProvider]) -> Bool) -> some View

Defines the destination of a drag-and-drop operation that handles the dropped content with a closure that you specify.

func onDrop(of: [UTType], isTargeted: Binding&lt;Bool>?, perform: ([NSItemProvider], CGPoint) -> Bool) -> some View

Defines the destination of a drag and drop operation that handles the dropped content with a closure that you specify.

