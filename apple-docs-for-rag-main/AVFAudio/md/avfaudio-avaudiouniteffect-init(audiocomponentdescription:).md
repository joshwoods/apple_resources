

- AVFAudio
- AVAudioUnitEffect
-  init(audioComponentDescription:) 

Initializer

# init(audioComponentDescription:)

Creates an audio unit effect object with the specified description.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
init(audioComponentDescription: AudioComponentDescription)
```

## Parameters 

`audioComponentDescription`  

The description of the audio unit to create.

The `audioComponentDescription` must be one of these types `kAudioUnitType_Effect`, `kAudioUnitType_MusicEffect`, `kAudioUnitType_Panner`, `kAudioUnitType_RemoteEffect`, or `kAudioUnitType_RemoteMusicEffect`.

## Return Value

A new `AVAudioUnitEffect` instance.

