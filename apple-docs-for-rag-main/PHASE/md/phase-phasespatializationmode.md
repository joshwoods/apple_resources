

- PHASE
-  PHASESpatializationMode 

Enumeration

# PHASESpatializationMode

The manner in which PHASE outputs spatial audio.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
enum PHASESpatializationMode
```

## Overview

When your app outputs audio through a spatial mixer, PHASESpatialMixerDefinition, the PHASE engine requires your app to choose an option of this enumeration and assign it to the outputSpatializationMode property.

## Topics

### Modes

case automatic

A mode that indicates that the framework chooses the spatialization mode.

case alwaysUseBinaural

A mode that introduces special processing to replicate a realistic spatial listening experience.

case alwaysUseChannelBased

A mode that adds a 3D position and orientation to sound by panning across the available output channels.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Setup

class PHASEEngine

An object that manages audio assets, controls playback, and configures environmental effects.

enum UpdateMode

Modes that determine when the framework consumes API calls and updates internal state.

class PHASEAssetRegistry

A central repository of audio assets.

enum PHASENormalizationMode

Options that determine whether the framework adjusts a sound asset’s loudness for the user’s output device.

enum PHASEReverbPreset

The manner in which PHASE diffuses resonating sound.

class PHASEMedium

A property or quality of the environment that affects how sound travels.

