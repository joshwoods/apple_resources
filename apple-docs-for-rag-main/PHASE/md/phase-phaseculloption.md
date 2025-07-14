

- PHASE
-  PHASECullOption 

Enumeration

# PHASECullOption

The actions the engine takes when it culls sound.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
enum PHASECullOption
```

## Overview

Culling refers to the temporary removal of a sound from the audio output. This enumeration determines the actions a sampler node performs after the engine culls its sound or queues it for culling. To indicate a preference, the app sets a sampler node’s cullOption property.

## Topics

### Options

case terminate

An option that culls sound by stopping playback.

case doNotCull

An option that indicates the framework takes no action to cull sound.

case sleepWakeAtRealtimeOffset

An option that pauses playback and resumes where it left off.

case sleepWakeAtZero

An option that pauses playback and resumes at the beginning.

case sleepWakeAtRandomOffset

An option that pauses playback and resumes at a random position.

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

### Defining Cull Behavior

var cullOption: PHASECullOption

The action the engine performs after it temporarily removes the node’s sound from the audio output.

