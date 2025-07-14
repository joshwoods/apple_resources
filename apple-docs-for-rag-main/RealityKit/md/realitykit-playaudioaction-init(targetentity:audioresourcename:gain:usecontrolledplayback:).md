

- RealityKit
- PlayAudioAction
-  init(targetEntity:audioResourceName:gain:useControlledPlayback:) 

Initializer

# init(targetEntity:audioResourceName:gain:useControlledPlayback:)

Creates a new play audio action.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
init(
    targetEntity: ActionEntityResolution = .sourceEntity,
    audioResourceName: String,
    gain: Audio.Decibel = 0,
    useControlledPlayback: Bool = true
)
```

## Parameters 

`targetEntity`  

The entity to play the audio.

`audioResourceName`  

The name of the audio stored in audio library component of the target entity to start playing.

`gain`  

The individual gain in decibels of the audio.

`useControlledPlayback`  

Determines whether this action has control over the playback of the audio.

