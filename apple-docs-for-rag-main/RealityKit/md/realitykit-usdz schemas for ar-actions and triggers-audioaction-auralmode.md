

- RealityKit
- USD Assets
- 
  - USD Assets
- USDZ schemas for AR
- Actions and triggers
- AudioAction
-  auralMode 

Article

# auralMode

An option that controls the audio signal’s spacial dynamics.

## Overview

The default value is blank. Each instance of `AudioAction` must specify an auralMode.

### Aural Modes

`spatial`  
Plays the audio in 3D space at the position of the affected object. If the device doesn’t support spatial audio, it falls back to mono. For best results in `spatial` mode, supply audio files in mono.

`nonSpatial`  
Plays the audio without regard to the affected object’s 3D position. If the audio media contains any form of stereo or other multichannel sound, the runtime attempts to match this to the device’s output capabilities. Use this mode when an audio action doesn’t use the listener’s position to affect the music’s playback.

`ambient`  
Plays the audio in a spatial configuration that tracks rotation, but does not attenuate with distance.

### Declaration

```
uniform token auralMode
```

## See Also

### Properties

info:id

The action’s unique identifier.

affectedObjects

A list of prims that respond to the notification.

audio

The location of an audio file.

type

An option that controls the order in which the actions execute.

gain

A value that controls the audio volume.

