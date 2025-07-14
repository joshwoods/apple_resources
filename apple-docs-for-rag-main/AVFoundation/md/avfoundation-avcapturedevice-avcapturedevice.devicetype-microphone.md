

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.DeviceType
-  microphone 

Type Property

# microphone

A microphone device type.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+

``` source
static let microphone: AVCaptureDevice.DeviceType
```

## Discussion

In iOS and tvOS, the system only exposes one capture device of this type. The audio routing subsystem decides which physical microphone to use, be it a built-in microphone, a wired headset, or an external microphone. The microphone device’s localizedName changes as the audio subsystem switches to a different physical device.

## See Also

### Microphones

static let builtInMicrophone: AVCaptureDevice.DeviceType

A built-in microphone.

Deprecated

