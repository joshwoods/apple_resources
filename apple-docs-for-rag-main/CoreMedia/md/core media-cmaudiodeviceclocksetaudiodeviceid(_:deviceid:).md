

- Core Media
-  CMAudioDeviceClockSetAudioDeviceID(\_:deviceID:) 

Function

# CMAudioDeviceClockSetAudioDeviceID(\_:deviceID:)

Changes the Core Audio device the clock is tracking by specifying a new device identifier.

macOS 10.8+

``` source
func CMAudioDeviceClockSetAudioDeviceID(
    _ clock: CMClock,
    deviceID: AudioDeviceID
) -> OSStatus
```

## Parameters 

`clock`  

The clock to change.

`deviceID`  

The new Core Audio device to track.

## See Also

### Configuring Audio Clocks

func CMAudioDeviceClockGetAudioDevice(CMClock, deviceUIDOut: AutoreleasingUnsafeMutablePointer&lt;CFString?>?, deviceIDOut: UnsafeMutablePointer&lt;AudioDeviceID>?, trackingDefaultDeviceOut: UnsafeMutablePointer&lt;DarwinBoolean>?) -> OSStatus

Returns the Core Audio device the clock is tracking.

func CMAudioDeviceClockSetAudioDeviceUID(CMClock, deviceUID: CFString?) -> OSStatus

Changes the Core Audio device the clock is tracking by specifying a new device unique identifier.

