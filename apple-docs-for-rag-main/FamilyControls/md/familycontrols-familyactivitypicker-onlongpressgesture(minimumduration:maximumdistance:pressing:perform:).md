

- FamilyControls
- FamilyActivityPicker
-  onLongPressGesture(minimumDuration:maximumDistance:pressing:perform:) 

Instance Method

# onLongPressGesture(minimumDuration:maximumDistance:pressing:perform:)

Adds an action to perform when this view recognizes a long press gesture.

FamilyControlsSwiftUIiOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.0–18.4DeprecatedmacOS 10.15–15.4DeprecatedvisionOSwatchOS 6.0–11.4Deprecated

``` source
nonisolated
func onLongPressGesture(
    minimumDuration: Double = 0.5,
    maximumDistance: CGFloat = 10,
    pressing: ((Bool) -> Void)? = nil,
    perform action: @escaping () -> Void
) -> some View
```

## See Also

### Deprecated Input and Event Modifiers

func onLongPressGesture(minimumDuration: Double, pressing: ((Bool) -> Void)?, perform: () -> Void) -> some View

Adds an action to perform when this view recognizes a long press gesture.

func onDrop(of: [String], delegate: any DropDelegate) -> some View

Defines the destination for a drag and drop operation with the same size and position as this view, with behavior controlled by the given delegate.

func onDrop(of: [String], isTargeted: Binding&lt;Bool>?, perform: ([NSItemProvider], CGPoint) -> Bool) -> some View

Defines the destination for a drag and drop operation with the same size and position as this view, handling dropped content and the drop location with the given closure.

func onDrop(of: [String], isTargeted: Binding&lt;Bool>?, perform: ([NSItemProvider]) -> Bool) -> some View

Defines the destination for a drag and drop operation, using the same size and position as this view, handling dropped content with the given closure.

