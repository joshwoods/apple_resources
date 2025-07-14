

- Audio Toolbox
- MusicTrackLoopInfo
-  init(loopDuration:numberOfLoops:) 

Initializer

# init(loopDuration:numberOfLoops:)

Initializes the music track loop information.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
init(
    loopDuration: MusicTimeStamp,
    numberOfLoops: Int32
)
```

## Parameters 

`loopDuration`  

The point in a music track, measured in beats from the end of the music track, at which to begin playback during looped playback. To explicitly turn off looping, specify a loopDuration of `0`.

`numberOfLoops`  

The number of times to play the designated portion of the music track. To loop forever, set numberOfLoops to `0`.

