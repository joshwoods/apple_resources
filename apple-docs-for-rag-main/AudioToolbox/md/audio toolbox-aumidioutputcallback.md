

- Audio Toolbox
-  AUMIDIOutputCallback 

Type Alias

# AUMIDIOutputCallback

When called by a host application, gets MIDI data from an audio unit.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias AUMIDIOutputCallback = (UnsafeMutableRawPointer?, UnsafePointer, UInt32, UnsafePointer) -> OSStatus
```

## Parameters 

`userData`  

Custom data.

`timeStamp`  

`midiOutNum`  

`pktlist`  

## Discussion

If you named your callback function `MyAUMIDIOutputCallback`, you would declare it like this:

## See Also

### Getting Information from the Host

typealias HostCallback_GetBeatAndTempo

When called by the system, provides beat and tempo information to an audio unit from a host application.

typealias HostCallback_GetMusicalTimeLocation

When called by the system, provides musical timing information to an audio unit from a host application.

typealias HostCallback_GetTransportState

When called by the system, provides audio transport state and timeline information to an audio unit from a host application.

typealias HostCallback_GetTransportState2

typealias AUInputSamplesInOutputCallback

Called by the system when an audio unit has provided a buffer of output samples.

