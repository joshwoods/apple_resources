

- PHASE
- PHASEEngine
-  PHASEEngine.UpdateMode 

Enumeration

# PHASEEngine.UpdateMode

Modes that determine when the framework consumes API calls and updates internal state.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
enum UpdateMode
```

## Overview

To define the manner in which PHASE processes commands and updates internal state, select an option from this enumeration and pass it to the `updateMode` parameter of the PHASEEngine initializer, init(updateMode:).

## Topics

### Modes

case automatic

A mode that indicates PHASE sets the timing of state adjustments.

case manual

A mode that indicates the app controls when the framework adjusts state.

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

class PHASEAssetRegistry

A central repository of audio assets.

enum PHASENormalizationMode

Options that determine whether the framework adjusts a sound asset’s loudness for the user’s output device.

enum PHASESpatializationMode

The manner in which PHASE outputs spatial audio.

enum PHASEReverbPreset

The manner in which PHASE diffuses resonating sound.

class PHASEMedium

A property or quality of the environment that affects how sound travels.

