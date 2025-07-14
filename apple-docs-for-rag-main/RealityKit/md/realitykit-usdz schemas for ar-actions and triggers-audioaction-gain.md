

- RealityKit
- USD Assets
- 
  - USD Assets
- USDZ schemas for AR
- Actions and triggers
- AudioAction
-  gain 

Article

# gain

A value that controls the audio volume.

## Overview

The runtime multiplies this value by the incoming audio to produce the output signal. An asset may use this action to raise or lower the audio’s original volume.

The default value of `1.0` matches the audio’s original volume. The runtime clamps negative values to `0.0`, which mutes the audio.

### Declaration

```
uniform double gain = 1.0
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

auralMode

An option that controls the audio signal’s spacial dynamics.

