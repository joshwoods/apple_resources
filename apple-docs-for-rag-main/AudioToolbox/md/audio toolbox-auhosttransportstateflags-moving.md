

- Audio Toolbox
- AUHostTransportStateFlags
-  moving 

Type Property

# moving

Indicates that the audio transport is moving.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
static var moving: AUHostTransportStateFlags { get }
```

## See Also

### Constants

static var changed: AUHostTransportStateFlags

Indicates such state changes as start, stop, or seeking to another position in the timeline. Can be active if there was a change to the state of, or discontinuities in, the audio transport since the AUHostTransportStateBlock callback was last called.

static var cycling: AUHostTransportStateFlags

Indicates that the host is cycling or looping.

static var recording: AUHostTransportStateFlags

Indicates that the host is recording, or is prepared to record. Can be active with or without a moving state.

