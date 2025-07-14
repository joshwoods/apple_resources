

- FamilyControls
- FamilyActivityPicker
-  onLongPressGesture(minimumDuration:pressing:perform:) 

Instance Method

# onLongPressGesture(minimumDuration:pressing:perform:)

Adds an action to perform when this view recognizes a long press gesture.

FamilyControlsSwiftUItvOS 14.0+

``` source
nonisolated
func onLongPressGesture(
    minimumDuration: Double = 0.5,
    pressing: ((Bool) -> Void)? = nil,
    perform action: @escaping () -> Void
) -> some View
```

## See Also

### Deprecated Input and Event Modifiers

func onLongPressGesture(minimumDuration: Double, maximumDistance: CGFloat, pressing: ((Bool) -> Void)?, perform: () -> Void) -> some View

Adds an action to perform when this view recognizes a long press gesture.

func onDrop(of: [String], delegate: any DropDelegate) -> some View

Defines the destination for a drag and drop operation with the same size and position as this view, with behavior controlled by the given delegate.

func onDrop(of: [String], isTargeted: Binding&lt;Bool>?, perform: ([NSItemProvider], CGPoint) -> Bool) -> some View

Defines the destination for a drag and drop operation with the same size and position as this view, handling dropped content and the drop location with the given closure.

func onDrop(of: [String], isTargeted: Binding&lt;Bool>?, perform: ([NSItemProvider]) -> Bool) -> some View

Defines the destination for a drag and drop operation, using the same size and position as this view, handling dropped content with the given closure.

