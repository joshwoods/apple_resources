

- AVFAudio
- AVAudioUnitGenerator
-  init(audioComponentDescription:) 

Initializer

# init(audioComponentDescription:)

Creates a generator audio unit with the specified description.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
init(audioComponentDescription: AudioComponentDescription)
```

## Parameters 

`audioComponentDescription`  

The audio component description.

## Return Value

A new `AVAudioUnitGenerator` instance.

## Discussion

The AudioComponentDescription structure `componentType` field must be `kAudioUnitType_Generator` or kAudioUnitType_RemoteGenerator.

