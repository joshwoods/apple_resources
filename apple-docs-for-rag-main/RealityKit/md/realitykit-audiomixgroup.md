

- RealityKit
-  AudioMixGroup 

Structure

# AudioMixGroup

A group that manages the playback properties of multiple playing sounds.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
struct AudioMixGroup
```

## Overview

A mix group component manages the playback parameters for a collection of different AudioPlaybackController and AudioGeneratorController instances. Properties such as gain, fade(to:duration:), and speed are multiplicative with the parameters you set on the controller.

You associate audio resources to a mix group by setting the `mixGroupName` parameter in the resource’s configuration. For an example, see mixGroupName. Enable a mix group by adding it to an AudioMixGroupsComponent structure on an entity in the scene. The scene where the component belongs limits the scope of the mix group.

```
var mixGroup = AudioMixGroup(name: "myMixGroup")
entity.components.set(AudioMixGroupsComponent(mixGroups: [mixGroup]))
```

## Topics

### Initializers

init(name: String)

Creates a mix group.

### Instance Properties

var gain: Audio.Decibel

The overall level for all sounds of an audio mix group in relative decibels.

var isMuted: Bool

A Boolean value that indicates whether an audio mix group emits any sound.

let name: String

The name of an audio mix group.

var speed: Double

The rate of playback for an audio mix group.

### Instance Methods

func fade(to: Audio.Decibel, duration: TimeInterval)

Transitions the gain to a value over a time interval using a linear curve.

### Default Implementations

Equatable Implementations

Hashable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable

## See Also

### Audio mixing

struct AudioMixGroupsComponent

A component that provides functionality for controlling the playback of audio you assign to mix groups in a scene.

