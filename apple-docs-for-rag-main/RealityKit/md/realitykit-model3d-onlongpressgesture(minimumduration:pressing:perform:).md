

- RealityKit
- Model3D
-  onLongPressGesture(minimumDuration:pressing:perform:) 

Instance Method

# onLongPressGesture(minimumDuration:pressing:perform:)

Adds an action to perform when this view recognizes a long press gesture.

RealityKitSwiftUItvOS 14.0+

``` source
nonisolated
func onLongPressGesture(
    minimumDuration: Double = 0.5,
    pressing: ((Bool) -> Void)? = nil,
    perform action: @escaping () -> Void
) -> some View
```

