

- Core Media
- CMClock
-  setAudioDeviceUID(\_:) 

Instance Method

# setAudioDeviceUID(\_:)

Sets the audio device by using the unique device identifier.

Mac Catalyst 13.0+macOS 10.15+

``` source
func setAudioDeviceUID(_ deviceUID: String?) throws
```

## Parameters 

`deviceUID`  

The device identifier.

## See Also

### Getting Time and Devices

func anchorTime() throws -> (anchorTime: CMTime, referenceTime: CMTime)

Returns the current time from a clock and the matching time from the clock’s reference clock.

func audioDevice() throws -> (deviceUID: String?, deviceID: AudioDeviceID, trackingDefaultDevice: Bool)

Returns the audio device the clock tracks.

func setAudioDeviceID(AudioDeviceID) throws

Sets the audio device by using the device identifier.

