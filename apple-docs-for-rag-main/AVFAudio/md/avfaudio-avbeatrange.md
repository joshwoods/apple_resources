

- AVFAudio
-  AVBeatRange 

Type Alias

# AVBeatRange

A specific time range within a music track.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias AVBeatRange = _AVBeatRange
```

## Topics

### Creating a Beat Range

func AVMakeBeatRange(AVMusicTimeStamp, AVMusicTimeStamp) -> AVBeatRange

Creates a beat range with the specified start time and length.

## See Also

### Handling Beat Range

func beats(forHostTime: UInt64, error: NSErrorPointer) -> AVMusicTimeStamp

Gets the beat the system plays at the specified host time.

func beats(forSeconds: TimeInterval) -> AVMusicTimeStamp

Gets the beat position (timestamp) for the specified time in the track.

var AVMusicTimeStampEndOfTrack: Double

A timestamp you use to access all events in a music track through a beat range.

