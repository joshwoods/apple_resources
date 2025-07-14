

- AVFAudio
-  AVMusicTimeStampEndOfTrack 

Global Variable

# AVMusicTimeStampEndOfTrack

A timestamp you use to access all events in a music track through a beat range.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var AVMusicTimeStampEndOfTrack: Double { get }
```

## Discussion

Pass this value as the length of an AVBeatRange to indicate an end time beyond the last event in the track. This makes it possible to specify a beat range that includes all events starting at a particular time, up to and including the last event.

## See Also

### Handling Beat Range

func beats(forHostTime: UInt64, error: NSErrorPointer) -> AVMusicTimeStamp

Gets the beat the system plays at the specified host time.

func beats(forSeconds: TimeInterval) -> AVMusicTimeStamp

Gets the beat position (timestamp) for the specified time in the track.

typealias AVBeatRange

A specific time range within a music track.

