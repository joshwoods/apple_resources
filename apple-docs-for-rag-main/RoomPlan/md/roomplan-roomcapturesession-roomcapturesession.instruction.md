

- RoomPlan
- RoomCaptureSession
-  RoomCaptureSession.Instruction 

Enumeration

# RoomCaptureSession.Instruction

Capture user instructions

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 16.0–1.0Deprecated

``` source
enum Instruction
```

## Mentioned in 

Scanning the rooms of a single structure

## Topics

### Determining a coaching recommendation

case normal

An instruction that indicates scanning proceeds normally and the user needs no coaching.

case moveCloseToWall

An instruction that requests the user move closer to the wall.

case moveAwayFromWall

An instruction that requests the user move further from the wall.

case turnOnLight

An instruction that requests the user increase the amount of light in the room.

case slowDown

An instruction that requests that the user move slower.

case lowTexture

An instruction that indicates the framework doesn’t detect distinguishable room features.

### Comparing instructions

static func == (RoomCaptureSession.Instruction, RoomCaptureSession.Instruction) -> Bool

Determines whether two instructions are equal.

static func != (Self, Self) -> Bool

Determines whether two instructions aren’t equal.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

var hashValue: Int

The hash value.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable

