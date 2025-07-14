

- Audio Toolbox
-  HostCallback_GetTransportState 

Type Alias

# HostCallback_GetTransportState

When called by the system, provides audio transport state and timeline information to an audio unit from a host application.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias HostCallback_GetTransportState = (UnsafeMutableRawPointer?, UnsafeMutablePointer?, UnsafeMutablePointer?, UnsafeMutablePointer?, UnsafeMutablePointer?, UnsafeMutablePointer?, UnsafeMutablePointer?) -> OSStatus
```

## Parameters 

`inHostUserData`  

Custom data that you provided when registering your callback with the audio unit.

`outIsPlaying`  

On output, `TRUE` if audio is playing, or `FALSE` otherwise.

`outTransportStateChanged`  

On output, `TRUE` if the transport state changed since the last time the callback was invoked, or `FALSE` otherwise.

`outCurrentSampleInTimeLine`  

On output, the sample number, indexed from zero from the beginning of the timeline.

`outIsCycling`  

On output, `TRUE` if cycling, or `FALSE` otherwise.

`outCycleStartBeat`  

`outCycleEndBeat`  

## Discussion

If you named your callback function `MyHostCallback_GetTransportState`, you would declare it like this:

## See Also

### Getting Information from the Host

typealias HostCallback_GetBeatAndTempo

When called by the system, provides beat and tempo information to an audio unit from a host application.

typealias HostCallback_GetMusicalTimeLocation

When called by the system, provides musical timing information to an audio unit from a host application.

typealias HostCallback_GetTransportState2

typealias AUInputSamplesInOutputCallback

Called by the system when an audio unit has provided a buffer of output samples.

typealias AUMIDIOutputCallback

When called by a host application, gets MIDI data from an audio unit.

