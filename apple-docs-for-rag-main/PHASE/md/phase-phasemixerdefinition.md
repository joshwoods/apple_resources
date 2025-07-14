

- PHASE
-  PHASEMixerDefinition 

Class

# PHASEMixerDefinition

An object to initialize a mixer with a given configuration.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
class PHASEMixerDefinition
```

## Overview

A mixer combines multiple layers of audio to a single signal for transmission to the output device. The framework creates a mixer when you provide a mixer definition. Instead of creating an instance of this class, instantiate one of the mixer definition subclasses instead:

PHASEChannelMixerDefinition  
When your app outputs sound through a channel mixer, the framework maintains the channel configuration of the source audio. For example, the left and right channels of a stereo input file play on the left and right speakers, respectively.

PHASEAmbientMixerDefinition  
When your app outputs sound through an ambient mixer, the framework overrides the output channels to give the mixer an orientation, which creates the effect of pointing in a specific direction in 3D space.

PHASESpatialMixerDefinition  
Audio that your app outputs through a spatial mixer specifies a position and orientation in 3D space. Spatial mixers require the app to define sources that emit audio, and a listener that hears audio. Sound playback changes depending on the relative positions of the listener and sources.

### Play a Sound Using a Mixer

To play a sound using a mixer, create a mixer definition and pass it to a sound event. The following code creates a PHASEChannelMixerDefinition and passes it into a node definition the app can invoke to play the channel-based audio file `drumloopSoundAsset`:

```
// Create a channel mixer definition.
let stereoMixer = PHASEChannelMixerDefinition(channelLayout:stereoLayout!)

// Pass the mixer to a sound event node definition that plays an audio file.
let drumloopSamplerNode = PHASESamplerNodeDefinition(soundAssetIdentifier:drumloopSoundAsset.identifier, mixerDefinition:stereoMixer, identifier:"drumloopNode")
```

## Topics

### Controlling Volume

var gain: Double

The mixer’s volume.

var gainMetaParameterDefinition: PHASENumberMetaParameterDefinition?

A template for a parameter that changes the mixer’s volume gradually over a period of time.

## Relationships

### Inherits From

- PHASEDefinition

### Inherited By

- PHASEAmbientMixerDefinition
- PHASEChannelMixerDefinition
- PHASESpatialMixerDefinition

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

class PHASEMixer

An object that combines multiple audio signals into a single signal.

class PHASEDefinition

A base class that adds a name to framework definitions.

Spatial Mixing

Define environmental characteristics that determine how sound plays in your app’s 3D soundscape.

