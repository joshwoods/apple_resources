

- Audio Toolbox
-  HostCallbackInfo 

Structure

# HostCallbackInfo

The time- and transport-related callback functions for an audio unit.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct HostCallbackInfo
```

## Topics

### Initializers

init()

init(hostUserData: UnsafeMutableRawPointer?, beatAndTempoProc: HostCallback_GetBeatAndTempo?, musicalTimeLocationProc: HostCallback_GetMusicalTimeLocation?, transportStateProc: HostCallback_GetTransportState?, transportStateProc2: HostCallback_GetTransportState2?)

### Instance Properties

var beatAndTempoProc: HostCallback_GetBeatAndTempo?

Your callback function that provides beat and tempo information to an audio unit. May be `NULL`.

var hostUserData: UnsafeMutableRawPointer?

Custom data specified by your application. May be `NULL`.

var musicalTimeLocationProc: HostCallback_GetMusicalTimeLocation?

Your callback function that provides musical timeline information to an audio unit. May be `NULL`.

var transportStateProc: HostCallback_GetTransportState?

Your callback function that provides audio transport state information (*play*, *rewind*, and so on) to an audio unit. May be `NULL`.

var transportStateProc2: HostCallback_GetTransportState2?

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### General

Other Plug-In Formats

RenderQuality

Render quality settings for audio units.

General Audio Unit Properties

Properties that apply to any audio unit.

