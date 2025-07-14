

- Core Media
- CMClock
-  anchorTime() 

Instance Method

# anchorTime()

Returns the current time from a clock and the matching time from the clock’s reference clock.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func anchorTime() throws -> (anchorTime: CMTime, referenceTime: CMTime)
```

## See Also

### Getting Time and Devices

func audioDevice() throws -> (deviceUID: String?, deviceID: AudioDeviceID, trackingDefaultDevice: Bool)

Returns the audio device the clock tracks.

func setAudioDeviceID(AudioDeviceID) throws

Sets the audio device by using the device identifier.

func setAudioDeviceUID(String?) throws

Sets the audio device by using the unique device identifier.

