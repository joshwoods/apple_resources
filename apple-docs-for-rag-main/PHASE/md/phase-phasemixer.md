

- PHASE
-  PHASEMixer 

Class

# PHASEMixer

An object that combines multiple audio signals into a single signal.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
class PHASEMixer
```

## Overview

Mixers provide a single point of control over the multiple audio signals they combine. To create a mixer, you provide the framework with a mixer definition; see PHASEMixerDefinition.

Subclasses of this class define unique properties the app sets to control specific features. For example, the spatial mixer (PHASESpatialMixerDefinition) adds environmental effects into the output audio signal.

## Topics

### Adjusting Volume

var gain: Double

The mixer’s volume.

var gainMetaParameter: PHASEMetaParameter?

A parameter that changes the mixer’s volume gradually over a period of time.

### Retrieving the Mixer Identifier

var identifier: String

A unique name for the mixer.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Audio Layering and Effects

class PHASEChannelMixerDefinition

An audio-layering object that routes sound directly to the device’s output.

class PHASEAmbientMixerDefinition

An audio-layering object that outputs sound in a particular direction in 3D space.

class PHASEMixerDefinition

An object to initialize a mixer with a given configuration.

class PHASEDefinition

A base class that adds a name to framework definitions.

Spatial Mixing

Define environmental characteristics that determine how sound plays in your app’s 3D soundscape.

