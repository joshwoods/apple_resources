

- Audio Toolbox
-  HostCallback_GetMusicalTimeLocation 

Type Alias

# HostCallback_GetMusicalTimeLocation

When called by the system, provides musical timing information to an audio unit from a host application.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias HostCallback_GetMusicalTimeLocation = (UnsafeMutableRawPointer?, UnsafeMutablePointer?, UnsafeMutablePointer?, UnsafeMutablePointer?, UnsafeMutablePointer?) -> OSStatus
```

## Parameters 

`inHostUserData`  

Custom data that you provided when registering your callback with the audio unit.

`outDeltaSampleOffsetToNextBeat`  

On output, the number of samples until the next beat.

`outTimeSig_Numerator`  

On output, the numerator for a musical time signature.

`outTimeSig_Denominator`  

On output, the denominator for a musical time signature.

`outCurrentMeasureDownBeat`  

## Discussion

If you named your callback function `MyHostCallback_GetMusicalTimeLocation`, you would declare it like this:

## See Also

### Getting Information from the Host

typealias HostCallback_GetBeatAndTempo

When called by the system, provides beat and tempo information to an audio unit from a host application.

typealias HostCallback_GetTransportState

When called by the system, provides audio transport state and timeline information to an audio unit from a host application.

typealias HostCallback_GetTransportState2

typealias AUInputSamplesInOutputCallback

Called by the system when an audio unit has provided a buffer of output samples.

typealias AUMIDIOutputCallback

When called by a host application, gets MIDI data from an audio unit.

