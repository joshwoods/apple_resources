

- FamilyControls
- FamilyActivityPicker
-  onDrop(of:delegate:) 

Instance Method

# onDrop(of:delegate:)

Defines the destination for a drag and drop operation with the same size and position as this view, with behavior controlled by the given delegate.

FamilyControlsSwiftUIiOS 13.4–18.4DeprecatediPadOS 13.4–18.4DeprecatedMac Catalyst 13.4–18.4DeprecatedmacOS 10.15–15.4DeprecatedvisionOS 1.0+

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

## See Also

### Deprecated Input and Event Modifiers

func onLongPressGesture(minimumDuration: Double, maximumDistance: CGFloat, pressing: ((Bool) -> Void)?, perform: () -> Void) -> some View

Adds an action to perform when this view recognizes a long press gesture.

func onLongPressGesture(minimumDuration: Double, pressing: ((Bool) -> Void)?, perform: () -> Void) -> some View

Adds an action to perform when this view recognizes a long press gesture.

func onDrop(of: [String], isTargeted: Binding&lt;Bool>?, perform: ([NSItemProvider], CGPoint) -> Bool) -> some View

Defines the destination for a drag and drop operation with the same size and position as this view, handling dropped content and the drop location with the given closure.

func onDrop(of: [String], isTargeted: Binding&lt;Bool>?, perform: ([NSItemProvider]) -> Bool) -> some View

Defines the destination for a drag and drop operation, using the same size and position as this view, handling dropped content with the given closure.

