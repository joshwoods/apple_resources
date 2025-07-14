

- RealityKit
- ARView
- ARView.Environment
- ARView.Environment.Reverb
-  ARView.Environment.Reverb.Preset 

Enumeration

# ARView.Environment.Reverb.Preset

Available reverb preset values.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+

``` source
enum Preset
```

## Topics

### Reverb presets

case cathedral

Reverb that sounds like the inside of a cathedral.

case largeHall

Reverb that sounds like the inside of a large hall.

case largeRoom

Reverb that sounds like the inside of a large room.

case mediumHall

Reverb that sounds like the inside of a medium hall.

case mediumRoom

Reverb that sounds like the inside of a medium room.

case smallRoom

Reverb that sounds like the inside of a small room.

### Comparing reverb presets

static func == (ARView.Environment.Reverb.Preset, ARView.Environment.Reverb.Preset) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

var hashValue: Int

The hash value.

### Default Implementations

CaseIterable Implementations

Equatable Implementations

## Relationships

### Conforms To

- CaseIterable
- Copyable
- Equatable
- Hashable

## See Also

### Reverb presets

static var automatic: ARView.Environment.Reverb

The default reverb preset.

