

- SwiftUI
-  DigitalCrownRotationalSensitivity 

Enumeration

# DigitalCrownRotationalSensitivity

The amount of Digital Crown rotation needed to move between two integer numbers.

watchOS 6.0+

``` source
enum DigitalCrownRotationalSensitivity
```

## Overview

You may need to experiment to find the level of sensitivity that works for your use case.

## Topics

### Getting sensitivity options

case low

Low sensitivity.

case medium

Medium sensitivity.

case high

High sensitivity.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
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

struct DigitalCrownEvent

An event emitted when the user rotates the Digital Crown.

