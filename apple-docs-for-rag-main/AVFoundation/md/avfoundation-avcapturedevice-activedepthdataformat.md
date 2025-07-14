

- AVFoundation
- AVCaptureDevice
-  activeDepthDataFormat 

Instance Property

# activeDepthDataFormat

The currently active depth data format of the capture device.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var activeDepthDataFormat: AVCaptureDevice.Format? { get set }
```

## Mentioned in 

Capturing Photos with Depth

## Discussion

You must obtain exclusive access to the device by calling lockForConfiguration() before setting this property value.

You can set this property only to formats present in the active format’s supportedDepthDataFormats array. Attempting to set an unsupported format throws an exception.

You can’t set the frame rate of depth data directly. Instead, the system synchronizes the depth data frame rate to the device’s activeVideoMinFrameDuration and activeVideoMaxFrameDuration values. It may match the device’s current frame rate, or lower, if the system can’t produce depth data fast enough for the active video frame rate.

Delivery of depth data to a AVCaptureDepthDataOutput may increase the system load, resulting in a reduced video frame rate for thermal sustainability.

On devices where depth data isn’t supported, this property value is `nil`.

This property is key-value observable.

## See Also

### Configuring Capture Formats

var formats: [AVCaptureDevice.Format]

The capture formats a device supports.

var activeFormat: AVCaptureDevice.Format

The capture format in use by the device.

class Format

A class that defines media formats and capture settings that capture devices support.

