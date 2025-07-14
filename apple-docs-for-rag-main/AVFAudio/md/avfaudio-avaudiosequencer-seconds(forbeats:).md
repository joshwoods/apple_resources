

- AVFAudio
- AVAudioSequencer
-  seconds(forBeats:) 

Instance Method

# seconds(forBeats:)

Gets the time for the specified beat position (timestamp) in the track, in seconds.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func seconds(forBeats beats: AVMusicTimeStamp) -> TimeInterval
```

## Parameters 

`beats`  

The timestamp for the beat position.

## See Also

### Managing Time Stamps

typealias AVMusicTimeStamp

A fractional number of beats.

func hostTime(forBeats: AVMusicTimeStamp, error: NSErrorPointer) -> UInt64

Gets the host time the sequence plays at the specified position.

