

- AVFAudio
-  AVMakeBeatRange(\_:\_:) 

Function

# AVMakeBeatRange(\_:\_:)

Creates a beat range with the specified start time and length.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func AVMakeBeatRange(
    _ startBeat: AVMusicTimeStamp,
    _ lengthInBeats: AVMusicTimeStamp
) -> AVBeatRange
```

## Parameters 

`startBeat`  

The timestamp for the start position.

`lengthInBeats`  

The length of the beat range, in beats.

