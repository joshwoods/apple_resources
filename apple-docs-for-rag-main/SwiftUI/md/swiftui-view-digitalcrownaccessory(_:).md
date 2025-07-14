

- SwiftUI
- View
-  digitalCrownAccessory(\_:) 

Instance Method

# digitalCrownAccessory(\_:)

Specifies the visibility of Digital Crown accessory Views on Apple Watch.

watchOS 9.0+

``` source
nonisolated
func digitalCrownAccessory(_ visibility: Visibility) -> some View
```

## Parameters 

`visibility`  

The visibility of the digital crown accessory.

## Discussion

Use this method to customize the visibility of a Digital Crown accessory `View` created with the `View/digitalCrownAccessory(_ content:)` modifier. You may want to keep an accessory visible even when the Digital Crown Indicator is not visible to indicate what scrolling the crown will do.

## See Also

### Interacting with the Digital Crown

func digitalCrownAccessory&lt;Content>(content: () -> Content) -> some View

Places an accessory View next to the Digital Crown on Apple Watch.

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

