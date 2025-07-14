

- RealityKit
- Reverb
-  Reverb.Preset 

Structure

# Reverb.Preset

Reverbs defined by a preset environment.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct Preset
```

## Topics

### Operators

static func == (Reverb.Preset, Reverb.Preset) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Properties

static let concertHall: Reverb.Preset

The reverb of a concert hall.

static let largeRoom: Reverb.Preset

The reverb of a large room.

static let largeRoomTreated: Reverb.Preset

The reverb of a large room with acoustical treatment.

static let mediumRoomDry: Reverb.Preset

The reverb of a medium-sized room with a significant amount of acoustical treatment.

static let mediumRoomTreated: Reverb.Preset

The reverb of a medium-sized room with acoustic treatment.

static let outside: Reverb.Preset

The reverb of an outside environment.

static let smallRoom: Reverb.Preset

The reverb of a small room with furniture and other common household items.

static let smallRoomBright: Reverb.Preset

The reverb of a small room with reflective surfaces.

static let veryLargeRoom: Reverb.Preset

The reverb of a very large room.

static let verySmallRoomBright: Reverb.Preset

The reverb of a very small room with reflective surfaces.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Reverb

struct Reverb

The reverberation RealityKit applies to spatial audio sources.

struct ReverbComponent

A component that defines the reverberation of spatial audio sources.

