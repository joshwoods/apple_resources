

- AVFAudio
- AVAudioUnitTimeEffect
-  init(audioComponentDescription:) 

Initializer

# init(audioComponentDescription:)

Creates a time effect audio unit with the specified description.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
init(audioComponentDescription: AudioComponentDescription)
```

## Parameters 

`audioComponentDescription`  

The description of the audio unit to create.

## Return Value

A new `AVAudioUnitTimeEffect` instance.

## Discussion

The `componentType` field of the description structure must be `kAudioUnitType_FormatConverter` (”`aufc`”); otherwise, the method raises an exception.

