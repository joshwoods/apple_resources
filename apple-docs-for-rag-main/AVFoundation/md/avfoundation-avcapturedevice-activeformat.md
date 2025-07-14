

- AVFoundation
- AVCaptureDevice
-  activeFormat 

Instance Property

# activeFormat

The capture format in use by the device.

iOS 7.0+iPadOS 7.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+visionOS 1.0+

``` source
var activeFormat: AVCaptureDevice.Format { get set }
```

## Discussion

In iOS, a device’s active format and a capture session’s sessionPreset are mutually exclusive. If you set a device’s active format, the session to which it’s attached changes its preset to inputPriority. Likewise if you set a preset on a capture session, the session assumes control of its input devices, and configures their active format appropriately.

Note

Audio devices don’t expose any user-configurable formats in iOS. To configure audio input on iOS, use AVAudioSession and its related APIs instead.

Set the activeFormat, activeVideoMinFrameDuration, and activeVideoMaxFrameDuration properties simultaneously by performing the configuration between calls to the session’s beginConfiguration() and commitConfiguration() methods.

```
// Configure capture session.
captureSession.beginConfiguration()

do {
    try device.lockForConfiguration()

    // Set the device's active format.
    device.activeFormat = // a supported format.

    // Set the device's min/max frame duration.
    device.activeVideoMinFrameDuration = // a supported minimum duration.
    device.activeVideoMaxFrameDuration = // a supported maximum duration.

    device.unlockForConfiguration()
} catch {
    // Handle error.
}

// Apply the changes to the session.
captureSession.commitConfiguration()
```

If you configure a session to use an active format intended for high resolution still photography, and you apply zoom, orientation, or format changes to an AVCaptureVideoDataOutput, the system may not meet the target framerate.

This property is key-value observable.

## See Also

### Configuring Capture Formats

var formats: [AVCaptureDevice.Format]

The capture formats a device supports.

var activeDepthDataFormat: AVCaptureDevice.Format?

The currently active depth data format of the capture device.

class Format

A class that defines media formats and capture settings that capture devices support.

