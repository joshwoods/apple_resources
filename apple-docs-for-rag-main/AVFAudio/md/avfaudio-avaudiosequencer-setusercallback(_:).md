

- AVFAudio
- AVAudioSequencer
-  setUserCallback(\_:) 

Instance Method

# setUserCallback(\_:)

Adds a callback that the sequencer calls each time it encounters a user event during playback.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func setUserCallback(_ userCallback: AVAudioSequencerUserCallback?)
```

## Parameters 

`userCallback`  

The user callback that the system calls.

## Discussion

The system calls the same callback for events that occur on any track in the sequencer. Set the callback to `nil` to disable it.

## See Also

### Setting the User Callback

typealias AVAudioSequencerUserCallback

A callback the sequencer calls asynchronously during playback when it encounters a user event.

