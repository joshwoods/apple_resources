

- RealityKit
- AudioResource
-  AudioResource.InputMode Deprecated

Enumeration

# AudioResource.InputMode

iOS 13.0–16.3DeprecatediPadOS 13.0–16.3DeprecatedMac Catalyst 13.0–16.3DeprecatedmacOS 10.15–13.3Deprecated

``` source
enum InputMode
```

Deprecated

Use the ChannelAudioComponent, AmbientAudioComponent, or SpatialAudioComponent instead.

## Topics

### Input modes

case nonSpatial

the input channels are mixed to whatever the output format is without any spatialization

case spatial

a spatialized with all degrees of freedom. This treats a resource as a mono stream so mixes all its channels to mono

case ambient

spatialized but ignores listener translation and only follows listener head rotation

### Comparing input modes

static func == (AudioResource.InputMode, AudioResource.InputMode) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

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

## See Also

### Deprecated

var inputMode: AudioResource.InputModeDeprecated

