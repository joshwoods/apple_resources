

- AVFoundation
- Capture setup
- AVCaptureDevice
-  Formats 

API Collection

# Formats

Configure capture formats and camera frame rates.

## Overview

The following code example illustrates how to select an iOS device’s highest possible frame rate:

```
func configureCameraForHighestFrameRate(device: AVCaptureDevice) {

    var bestFormat: AVCaptureDevice.Format?
    var bestFrameRateRange: AVFrameRateRange?

    for format in device.formats {
        for range in format.videoSupportedFrameRateRanges {
            if range.maxFrameRate > bestFrameRateRange?.maxFrameRate ?? 0 {
                bestFormat = format
                bestFrameRateRange = range
            }
        }
    }

    if let bestFormat = bestFormat, 
       let bestFrameRateRange = bestFrameRateRange {
        do {
            try device.lockForConfiguration()

            // Set the device's active format.
            device.activeFormat = bestFormat

            // Set the device's min/max frame duration.
            let duration = bestFrameRateRange.minFrameDuration
            device.activeVideoMinFrameDuration = duration
            device.activeVideoMaxFrameDuration = duration

            device.unlockForConfiguration()
        } catch {
            // Handle error.
        }
    }
}
```

Most common configurations of capture settings are available through the AVCaptureSession object and its available presets. However, on iOS devices, some specialized options (such as high frame rate) require directly setting a capture format on an AVCaptureDevice instance.

Note

In iOS, directly configuring a capture device’s activeFormat property changes the capture session’s preset to inputPriority. Upon making this change, the capture session no longer automatically configures the capture format when you call the startRunning() method or call the commitConfiguration() method after changing the session topology.

In macOS, a capture session can still automatically configure the capture format after you make changes. To prevent automatic changes to the capture format in macOS, follow the advice listed under the lockForConfiguration() method.

## Topics

### Configuring Capture Formats

var formats: [AVCaptureDevice.Format]

The capture formats a device supports.

var activeFormat: AVCaptureDevice.Format

The capture format in use by the device.

var activeDepthDataFormat: AVCaptureDevice.Format?

The currently active depth data format of the capture device.

class Format

A class that defines media formats and capture settings that capture devices support.

### Configuring Frame Durations

var activeVideoMinFrameDuration: CMTime

The currently active minimum frame duration.

var activeVideoMaxFrameDuration: CMTime

The currently active maximum frame duration.

var activeDepthDataMinFrameDuration: CMTime

The minimum frame duration of depth data.

## See Also

### Configuring Camera Hardware

func lockForConfiguration() throws

Requests exclusive access to configure device hardware properties.

func unlockForConfiguration()

Releases exclusive control over device hardware properties.

var isSubjectAreaChangeMonitoringEnabled: Bool

A Boolean value that indicates whether the device monitors the subject area for changes.

class let subjectAreaDidChangeNotification: NSNotification.Name

A notification the system posts when a capture device detects a substantial change to the video subject area.

Focus

Configure the automatic focus behavior of a camera, or manually set its lens position.

Exposure

Configure the automatic exposure behavior of a camera, or manually control its exposure settings.

White Balance

Configure the automatic white balance behavior of a camera, or manually control white balance settings.

Lighting

Configure the device flash, torch, and low light settings.

Color

Manage HDR and color space settings for a device.

Zoom

Configure device zooming behavior and inspect hardware capabilities.

