

- AVFAudio
- AVAudioPlayerDelegate
-  audioPlayerDidFinishPlaying(\_:successfully:) 

Instance Method

# audioPlayerDidFinishPlaying(\_:successfully:)

Tells the delegate when the audio finishes playing.

iOS 2.2+iPadOS 2.2+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
optional func audioPlayerDidFinishPlaying(
    _ player: AVAudioPlayer,
    successfully flag: Bool
)
```

## Parameters 

`player`  

The audio player that finishes playing.

`flag`  

A Boolean value that indicates whether the audio finishes playing successfully.

## Discussion

The system doesn’t call this method on an audio interruption.

