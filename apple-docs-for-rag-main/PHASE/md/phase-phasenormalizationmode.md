

- PHASE
-  PHASENormalizationMode 

Enumeration

# PHASENormalizationMode

Options that determine whether the framework adjusts a sound asset’s loudness for the user’s output device.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
enum PHASENormalizationMode
```

## Overview

Different output devices feature loudness characteristics that require the audio engine to adjust the volume of the input audio to achieve a consistent listening experience across devices.

PHASE callibrates sound asset and stream loudness automatically when the app chooses PHASENormalizationMode.dynamic. If an app chooses PHASENormalizationMode.none, the app needs to implement custom loudness normalizaton manually, by adjusting sound asset and stream signal strength for the user’s output device.

## Topics

### Loudness Normalization Modes

case dynamic

A mode that instructs the framework to adjust a sound’s volume according to the user’s output device.

case none

A mode that instructs the framework not to adjust a sound’s volume according to the user’s output device.

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

enum PHASESpatializationMode

The manner in which PHASE outputs spatial audio.

enum PHASEReverbPreset

The manner in which PHASE diffuses resonating sound.

class PHASEMedium

A property or quality of the environment that affects how sound travels.

