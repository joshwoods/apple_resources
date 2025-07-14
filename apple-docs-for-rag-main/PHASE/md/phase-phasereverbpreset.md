

- PHASE
-  PHASEReverbPreset 

Enumeration

# PHASEReverbPreset

The manner in which PHASE diffuses resonating sound.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
enum PHASEReverbPreset
```

## Overview

The PHASE engine requires your app to choose an option of this enumeration and assign it to the defaultReverbPreset property.

The value you choose adds resonation to sound that simulates the experience of hearing it in a particular environment. For example, a small room, PHASEReverbPreset.smallRoom, adds very little reverberation compared to a large chamber, PHASEReverbPreset.largeChamber.

## Topics

### Presets

case cathedral

A resonation that simulates the experience of hearing a sound in a cathedral.

case largeChamber

A resonation that simulates the experience of hearing a sound in a large chamber with specific dimensions.

case largeHall

A resonation that simulates the experience of hearing a sound in a large hall with specific dimensions.

case largeHall2

A resonation that simulates the experience of hearing a sound in one kind of large hall with specific dimensions.

case largeRoom

A resonation that simulates the experience of hearing a sound in a large room with specific dimensions.

case largeRoom2

A resonation that simulates the experience of hearing a sound in one kind of large room with specific dimensions.

case mediumChamber

A resonation that simulates the experience of hearing a sound in a medium-size chamber with specific dimensions.

case mediumHall

A resonation that simulates the experience of hearing a sound in a medium-size hall with specific dimensions.

case mediumHall2

A resonation that simulates the experience of hearing a sound in one kind of medium-size hall with specific dimensions.

case mediumHall3

A resonation that simulates the experience of hearing a sound in another kind of medium-size hall with specific dimensions.

case mediumRoom

A resonation that simulates the experience of hearing a sound in a medium-size room with specific dimensions.

case none

An option that adds no reverberation to a sound.

case smallRoom

A resonation that simulates the experience of hearing a sound in a small room with specific dimensions.

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

enum PHASESpatializationMode

The manner in which PHASE outputs spatial audio.

class PHASEMedium

A property or quality of the environment that affects how sound travels.

