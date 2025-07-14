

- AVFAudio
- AVAudioPlayerDelegate
-  audioPlayerDecodeErrorDidOccur(\_:error:) 

Instance Method

# audioPlayerDecodeErrorDidOccur(\_:error:)

Tells the delegate when an audio player encounters a decoding error during playback.

iOS 2.2+iPadOS 2.2+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
optional func audioPlayerDecodeErrorDidOccur(
    _ player: AVAudioPlayer,
    error: (any Error)?
)
```

## Parameters 

`player`  

The audio player that encounters the decoding error.

`error`  

The decoding error.

