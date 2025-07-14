

- Audio Toolbox
-  HostCallback_GetTransportState2 

Type Alias

# HostCallback_GetTransportState2

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias HostCallback_GetTransportState2 = (UnsafeMutableRawPointer?, UnsafeMutablePointer?, UnsafeMutablePointer?, UnsafeMutablePointer?, UnsafeMutablePointer?, UnsafeMutablePointer?, UnsafeMutablePointer?, UnsafeMutablePointer?) -> OSStatus
```

## See Also

### Getting Information from the Host

typealias HostCallback_GetBeatAndTempo

When called by the system, provides beat and tempo information to an audio unit from a host application.

typealias HostCallback_GetMusicalTimeLocation

When called by the system, provides musical timing information to an audio unit from a host application.

typealias HostCallback_GetTransportState

When called by the system, provides audio transport state and timeline information to an audio unit from a host application.

typealias AUInputSamplesInOutputCallback

Called by the system when an audio unit has provided a buffer of output samples.

typealias AUMIDIOutputCallback

When called by a host application, gets MIDI data from an audio unit.

