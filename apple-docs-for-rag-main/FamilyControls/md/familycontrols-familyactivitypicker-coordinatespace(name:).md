

- FamilyControls
- FamilyActivityPicker
-  coordinateSpace(name:) 

Instance Method

# coordinateSpace(name:)

Assigns a name to the view’s coordinate space, so other code can operate on dimensions like points and sizes relative to the named space.

FamilyControlsSwiftUIiOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.0–18.4DeprecatedmacOS 10.15–15.4DeprecatedtvOS 13.0+visionOS 1.0+watchOS 6.0–11.4Deprecated

``` source
nonisolated
func coordinateSpace(name: T) -> some View where T : Hashable
```

## Parameters 

`name`  

A name used to identify this coordinate space.

## Discussion

Use `coordinateSpace(name:)` to allow another function to find and operate on a view and operate on dimensions relative to that view.

The example below demonstrates how a nested view can find and operate on its enclosing view’s coordinate space:

```
struct ContentView: View {
    @State private var location = CGPoint.zero

    var body: some View {
        VStack {
            Color.red.frame(width: 100, height: 100)
                .overlay(circle)
            Text("Location: \(Int(location.x)), \(Int(location.y))")
        }
        .coordinateSpace(name: "stack")
    }

    var circle: some View {
        Circle()
            .frame(width: 25, height: 25)
            .gesture(drag)
            .padding(5)
    }

    var drag: some Gesture {
        DragGesture(coordinateSpace: .named("stack"))
            .onChanged { info in location = info.location }
    }
}
```

Here, the `VStack` in the `ContentView` named “stack” is composed of a red frame with a custom `Circle` view `View/overlay(_:alignment:)` at its center.

The `circle` view has an attached `DragGesture` that targets the enclosing VStack’s coordinate space. As the gesture recognizer’s closure registers events inside `circle` it stores them in the shared `location` state variable and the `VStack` displays the coordinates in a `Text` view.

## See Also

### Position

func position(CGPoint) -> some View

Positions the center of this view at the specified point in its parent’s coordinate space.

func position(x: CGFloat, y: CGFloat) -> some View

Positions the center of this view at the specified coordinates in its parent’s coordinate space.

func offset(CGSize) -> some View

Offset this view by the horizontal and vertical amount specified in the offset parameter.

func offset(x: CGFloat, y: CGFloat) -> some View

Offset this view by the specified horizontal and vertical distances.

