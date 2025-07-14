

- AVFAudio
- AVAudioUnitMIDIInstrument
-  init(audioComponentDescription:) 

Initializer

# init(audioComponentDescription:)

Creates a MIDI instrument audio unit with the component description you specify.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
init(audioComponentDescription description: AudioComponentDescription)
```

## Parameters 

`description`  

The description of the audio component.

## Return Value

A new AVAudioUnitMIDIInstrument instance.

## Discussion

The component type must be `kAudioUnitType_MusicDevice` or `kAudioUnitType_RemoteInstrument`.

