

- AVFoundation
- AVAudioMixInputParameters
-  audioTapProcessor 

Instance Property

# audioTapProcessor

The audio processing tap associated with the track.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
var audioTapProcessor: MTAudioProcessingTap? { get }
```

## Discussion

You can use the audio tap to access the track’s audio data before it is played, read, or exported. This property is `nil` by default.

The process of setting up a tap requires the configuration of an instance of AVMutableAudioMixInputParameters. If an instance of AVMutableAudioMixInputParameters is present in the inputParameters array of an AVAudioMix, the results of mutating the AVMutableAudioMixInputParameters while the audio mix is in use are undefined

