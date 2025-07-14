

- Core Media
-  CMAudioDeviceClockSetAudioDeviceUID(\_:deviceUID:) 

Function

# CMAudioDeviceClockSetAudioDeviceUID(\_:deviceUID:)

Changes the Core Audio device the clock is tracking by specifying a new device unique identifier.

macOS 10.8+

``` source
func CMAudioDeviceClockSetAudioDeviceUID(
    _ clock: CMClock,
    deviceUID: CFString?
) -> OSStatus
```

## Parameters 

`clock`  

The clock to change.

`deviceUID`  

The UID of the Core Audio device to track.

## Discussion

Pass `NULL` for `deviceUID` to make the clock track the default device.

## See Also

### Configuring Audio Clocks

func CMAudioDeviceClockGetAudioDevice(CMClock, deviceUIDOut: AutoreleasingUnsafeMutablePointer&lt;CFString?>?, deviceIDOut: UnsafeMutablePointer&lt;AudioDeviceID>?, trackingDefaultDeviceOut: UnsafeMutablePointer&lt;DarwinBoolean>?) -> OSStatus

Returns the Core Audio device the clock is tracking.

func CMAudioDeviceClockSetAudioDeviceID(CMClock, deviceID: AudioDeviceID) -> OSStatus

Changes the Core Audio device the clock is tracking by specifying a new device identifier.

