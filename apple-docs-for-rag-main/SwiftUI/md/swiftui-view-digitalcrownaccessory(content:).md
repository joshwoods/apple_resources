

- SwiftUI
- View
-  digitalCrownAccessory(content:) 

Instance Method

# digitalCrownAccessory(content:)

Places an accessory View next to the Digital Crown on Apple Watch.

watchOS 9.0+

``` source
nonisolated
func digitalCrownAccessory(@ViewBuilder content: @escaping () -> Content) -> some View where Content : View
```

## Parameters 

`content`  

The view to be used as a Digital Crown Accessory.

## Discussion

Use this method to place a custom `View` next to the Digital Crown on Apple Watch. Use digitalCrownAccessory(_:) to specify the visibility of your custom view.

```
struct ZoomingMapView: View {
    // Width of the map displayed on screen in miles
    @State private var zoomLevel: Int = 1.0

    var body: some View {
        CustomMap(width: .miles(zoomLevel))
            .focusable()
            .digitalCrownRotation(value: $zoomLevel)
            .digitalCrownAccessory {
                Text("\(zoomLevel, specifier: "%.2f")MI")
                .background {
                    RoundedRectangle(cornerRadius: 5)
                        .fill(Color.gray)
                }
            }
    }
}
```

## See Also

### Interacting with the Digital Crown

func digitalCrownAccessory(Visibility) -> some View

Specifies the visibility of Digital Crown accessory Views on Apple Watch.

func digitalCrownRotation&lt;V>(Binding&lt;V>, from: V, through: V, sensitivity: DigitalCrownRotationalSensitivity, isContinuous: Bool, isHapticFeedbackEnabled: Bool, onChange: (DigitalCrownEvent) -> Void, onIdle: () -> Void) -> some View

Tracks Digital Crown rotations by updating the specified binding.

func digitalCrownRotation&lt;V>(Binding&lt;V>, onChange: (DigitalCrownEvent) -> Void, onIdle: () -> Void) -> some View

Tracks Digital Crown rotations by updating the specified binding.

func digitalCrownRotation(detent:from:through:by:sensitivity:isContinuous:isHapticFeedbackEnabled:onChange:onIdle:)

Tracks Digital Crown rotations by updating the specified binding.

func digitalCrownRotation&lt;V>(Binding&lt;V>) -> some View

Tracks Digital Crown rotations by updating the specified binding.

func digitalCrownRotation&lt;V>(Binding&lt;V>, from: V, through: V, by: V.Stride?, sensitivity: DigitalCrownRotationalSensitivity, isContinuous: Bool, isHapticFeedbackEnabled: Bool) -> some View

Tracks Digital Crown rotations by updating the specified binding.

struct DigitalCrownEvent

An event emitted when the user rotates the Digital Crown.

enum DigitalCrownRotationalSensitivity

The amount of Digital Crown rotation needed to move between two integer numbers.

