

- Audio Toolbox
- MusicTrackLoopInfo
-  loopDuration 

Instance Property

# loopDuration

The point in a music track, measured in beats from the end of the music track, at which to begin playback during looped playback.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var loopDuration: MusicTimeStamp
```

## Discussion

During looped playback, a music track plays from (`kSequenceTrackProperty_TrackLength` – `loopDuration`) to `kSequenceTrackProperty_TrackLength`.

To explicitly turn off looping, specify a loopDuration of `0`.

