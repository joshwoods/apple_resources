

- PHASE
-  PHASEMedium 

Class

# PHASEMedium

A property or quality of the environment that affects how sound travels.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
class PHASEMedium
```

## Overview

This class defines choices for the engine’s defaultMedium. Currently, this property provides only sound traveling through air.

## Topics

### Creating a Medium

init(engine: PHASEEngine, preset: PHASEMedium.Preset)

Creates a medium.

enum Preset

Predetermined qualities of an environment that affect how sound transmits.

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

### Setup

class PHASEEngine

An object that manages audio assets, controls playback, and configures environmental effects.

enum UpdateMode

Modes that determine when the framework consumes API calls and updates internal state.

class PHASEAssetRegistry

A central repository of audio assets.

enum PHASENormalizationMode

Options that determine whether the framework adjusts a sound asset’s loudness for the user’s output device.

enum PHASESpatializationMode

The manner in which PHASE outputs spatial audio.

enum PHASEReverbPreset

The manner in which PHASE diffuses resonating sound.

