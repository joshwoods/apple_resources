

- AVFoundation
- AVCaptureDevice
-  formats 

Instance Property

# formats

The capture formats a device supports.

iOS 7.0+iPadOS 7.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+visionOS 1.0+

``` source
var formats: [AVCaptureDevice.Format] { get }
```

## Discussion

A capture device format describes the details of the video, image, or audio parameters of a specific mode of capture. If you require specifying capture settings not covered by a capture session preset, you can set the activeFormat property to any of the formats in this array.

This property value is key-value observable.

## See Also

### Configuring Capture Formats

var activeFormat: AVCaptureDevice.Format

The capture format in use by the device.

var activeDepthDataFormat: AVCaptureDevice.Format?

The currently active depth data format of the capture device.

class Format

A class that defines media formats and capture settings that capture devices support.

