

- AVFAudio
-  AVAudioSequencerUserCallback 

Type Alias

# AVAudioSequencerUserCallback

A callback the sequencer calls asynchronously during playback when it encounters a user event.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
typealias AVAudioSequencerUserCallback = (AVMusicTrack, Data, AVMusicTimeStamp) -> Void
```

## Parameters 

`track`  

The track that contains the user event.

`userData`  

The data used to initialize the user event.

`timeStamp`  

The beat location of the event.

## Discussion

The sequencer delivers this callback asynchronously to the rendering thread on an internal queue. The `userData` this returns is unique to each AVMusicUserEvent instance.

## See Also

### Setting the User Callback

func setUserCallback(AVAudioSequencerUserCallback?)

Adds a callback that the sequencer calls each time it encounters a user event during playback.

