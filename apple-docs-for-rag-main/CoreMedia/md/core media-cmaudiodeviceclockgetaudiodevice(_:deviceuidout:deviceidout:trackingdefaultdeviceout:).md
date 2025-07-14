

- Core Media
-  CMAudioDeviceClockGetAudioDevice(\_:deviceUIDOut:deviceIDOut:trackingDefaultDeviceOut:) 

Function

# CMAudioDeviceClockGetAudioDevice(\_:deviceUIDOut:deviceIDOut:trackingDefaultDeviceOut:)

Returns the Core Audio device the clock is tracking.

macOS 10.8+

``` source
func CMAudioDeviceClockGetAudioDevice(
    _ clock: CMClock,
    deviceUIDOut: AutoreleasingUnsafeMutablePointer?,
    deviceIDOut: UnsafeMutablePointer?,
    trackingDefaultDeviceOut: UnsafeMutablePointer?
) -> OSStatus
```

## Parameters 

`clock`  

The clock from which to retrieve its audio device.

`deviceUIDOut`  

An optional unique device identifier. If you specify a non-`NULL` value, this function returns the `deviceUID` and its associated ID, and sets `trackingDefaultDeviceOut` to `false`.

`deviceIDOut`  

An optional device identifier. If you specify a non-`NULL` value, this function returns a `NULL` UID and the device ID, and sets `trackingDefaultDeviceOut` to `false`.

`trackingDefaultDeviceOut`  

On return, a Boolean value that indicates whether the audio clock tracks the default audio device.

## Return Value

A value that indicates the completion status.

## See Also

### Configuring Audio Clocks

func CMAudioDeviceClockSetAudioDeviceUID(CMClock, deviceUID: CFString?) -> OSStatus

Changes the Core Audio device the clock is tracking by specifying a new device unique identifier.

func CMAudioDeviceClockSetAudioDeviceID(CMClock, deviceID: AudioDeviceID) -> OSStatus

Changes the Core Audio device the clock is tracking by specifying a new device identifier.

