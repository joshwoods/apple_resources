

- Core Media
- CMClock
-  audioDevice() 

Instance Method

# audioDevice()

Returns the audio device the clock tracks.

Mac Catalyst 13.0+macOS 10.15+

``` source
func audioDevice() throws -> (deviceUID: String?, deviceID: AudioDeviceID, trackingDefaultDevice: Bool)
```

## See Also

### Getting Time and Devices

func anchorTime() throws -> (anchorTime: CMTime, referenceTime: CMTime)

Returns the current time from a clock and the matching time from the clock’s reference clock.

func setAudioDeviceID(AudioDeviceID) throws

Sets the audio device by using the device identifier.

func setAudioDeviceUID(String?) throws

Sets the audio device by using the unique device identifier.

