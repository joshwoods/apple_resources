

- Media Toolbox
-  MTAudioProcessingTapCreationFlags 

Type Alias

# MTAudioProcessingTapCreationFlags

Flags to use when creating audio processing taps.

iOS 6.0+iPadOS 6.0+Mac Catalyst 6.0+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
typealias MTAudioProcessingTapCreationFlags = UInt32
```

## Discussion

You must set the pre or post flag, but not both.

## Topics

### Flags

var kMTAudioProcessingTapCreationFlag_PreEffects: MTAudioProcessingTapCreationFlags

Signifies that the processing tap is inserted before any effects.

var kMTAudioProcessingTapCreationFlag_PostEffects: MTAudioProcessingTapCreationFlags

Signifies that the processing tap is inserted before any effects.

