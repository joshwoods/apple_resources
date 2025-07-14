

- RealityKit
- RealityViewAttachmentBuilderContent
-  onTapGesture(count:coordinateSpace:perform:) 

Instance Method

# onTapGesture(count:coordinateSpace:perform:)

Adds an action to perform when this view recognizes a tap gesture, and provides the action with the location of the interaction.

RealityKitSwiftUIiOS 16.0–18.4DeprecatediPadOS 16.0–18.4DeprecatedmacOS 13.0–15.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 9.0+

``` source
nonisolated
func onTapGesture(
    count: Int = 1,
    coordinateSpace: CoordinateSpace = .local,
    perform action: @escaping (CGPoint) -> Void
) -> some View
```

## Parameters 

`count`  

The number of taps or clicks required to trigger the action closure provided in `action`. Defaults to `1`.

`coordinateSpace`  

The coordinate space in which to receive location values. Defaults to `CoordinateSpace/local`.

`action`  

The action to perform. This closure receives an input that indicates where the interaction occurred.

## Discussion

Use this method to perform the specified `action` when the user clicks or taps on the modified view `count` times. The action closure receives the location of the interaction.

Note

If you create a control that’s functionally equivalent to a `Button`, use `ButtonStyle` to create a customized button instead.

The following code adds a tap gesture to a `Circle` that toggles the color of the circle based on the tap location.

```
struct TapGestureExample: View {
    @State private var location: CGPoint = .zero

    var body: some View {
        Circle()
            .fill(self.location.y > 50 ? Color.blue : Color.red)
            .frame(width: 100, height: 100, alignment: .center)
            .onTapGesture { location in
                self.location = location
            }
    }
}
```

