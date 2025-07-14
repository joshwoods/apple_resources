

- AVFAudio
-  AVMusicTimeStamp 

Type Alias

# AVMusicTimeStamp

A fractional number of beats.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias AVMusicTimeStamp = Double
```

## Discussion

Use this value for all sequencer timeline-related methods. The tempo of the sequence determines the relationship between this value and time (in seconds).

## See Also

### Managing Time Stamps

func hostTime(forBeats: AVMusicTimeStamp, error: NSErrorPointer) -> UInt64

Gets the host time the sequence plays at the specified position.

func seconds(forBeats: AVMusicTimeStamp) -> TimeInterval

Gets the time for the specified beat position (timestamp) in the track, in seconds.

