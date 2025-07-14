

- PHASE
-  PHASEChannelMixerDefinition 

Class

# PHASEChannelMixerDefinition

An audio-layering object that routes sound directly to the device’s output.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
class PHASEChannelMixerDefinition
```

## Overview

Use this class to play one-time sounds such as menu clicks.

Note

If your audio playback requires 3D orienting or positioning, use PHASEAmbientMixerDefinition or PHASESpatialMixerDefinition, respectively. For more information, see Spatial Mixing.

This class defines the *channel routing*, which is the strategy the framework uses to send source mono or multichannel assets to the output for playback. The asset’s audio channels route to the output for playback according to the channel layout and runtime output conditions the app designates on an instance of this class.

This class minimizes *up mixing* and *down mixing* — that is, source audio channel conversion to a higher or lower number of channels. For example, although a spatial mixer overrides the use of output channels by panning to convey listener position and orientation, the channel mixer maintains source audio channel layout to preserve the listening experience of the source audio.

## Topics

### Creating a Channel Mixer

init(channelLayout: AVAudioChannelLayout)

Creates a channel mixer with the given channel layout.

convenience init(channelLayout: AVAudioChannelLayout, identifier: String)

Creates a named channel mixer with the given channel layout.

### Inspecting Channel Layout

var inputChannelLayout: AVAudioChannelLayout

The channel layout of the mixer’s input audio.

## Relationships

### Inherits From

- PHASEMixerDefinition

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Audio Layering and Effects

class PHASEAmbientMixerDefinition

An audio-layering object that outputs sound in a particular direction in 3D space.

class PHASEMixerDefinition

An object to initialize a mixer with a given configuration.

class PHASEMixer

An object that combines multiple audio signals into a single signal.

class PHASEDefinition

A base class that adds a name to framework definitions.

Spatial Mixing

Define environmental characteristics that determine how sound plays in your app’s 3D soundscape.

