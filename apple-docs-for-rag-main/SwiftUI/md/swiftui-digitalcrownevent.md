

- SwiftUI
-  DigitalCrownEvent 

Structure

# DigitalCrownEvent

An event emitted when the user rotates the Digital Crown.

watchOS 9.0+

``` source
struct DigitalCrownEvent
```

## Overview

Use the digitalCrownRotation(_:) modifier to receive these events.

## Topics

### Getting events

var offset: Double

The offset of the digital crown when this event was sent.

var velocity: Double

The velocity at which the offset was changing when this event was sent.

## Relationships

### Conforms To

- Sendable

## See Also

### Interacting with the Digital Crown

func digitalCrownAccessory(Visibility) -> some View

Specifies the visibility of Digital Crown accessory Views on Apple Watch.

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

enum DigitalCrownRotationalSensitivity

The amount of Digital Crown rotation needed to move between two integer numbers.

