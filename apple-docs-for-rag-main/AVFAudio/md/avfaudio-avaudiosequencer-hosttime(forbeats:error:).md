

- AVFAudio
- AVAudioSequencer
-  hostTime(forBeats:error:) 

Instance Method

# hostTime(forBeats:error:)

Gets the host time the sequence plays at the specified position.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func hostTime(
    forBeats inBeats: AVMusicTimeStamp,
    error outError: NSErrorPointer
) -> UInt64
```

## Parameters 

`inBeats`  

The timestamp for the beat position.

`outError`  

On exit, if an error occurs, a description of the error.

## Discussion

This call is valid when the player is in a playing state. It returns `0` with an error, otherwise, or if the starting position of the player is after the specified beat. The method uses the sequence’s tempo map to translate a beat time from the starting time and the beat of the player.

## See Also

### Managing Time Stamps

typealias AVMusicTimeStamp

A fractional number of beats.

func seconds(forBeats: AVMusicTimeStamp) -> TimeInterval

Gets the time for the specified beat position (timestamp) in the track, in seconds.

