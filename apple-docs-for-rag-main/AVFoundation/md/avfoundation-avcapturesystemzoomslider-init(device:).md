

- AVFoundation
- AVCaptureSystemZoomSlider
-  init(device:) 

Initializer

# init(device:)

Creates a slider to control the video zoom factor of a capture device.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+

``` source
init(device: AVCaptureDevice)
```

## Parameters 

`device`  

The capture device to control.

## Discussion

You can only create a zoom slider with a device that support’s setting its videoZoomFactor property value.

## See Also

### Creating a zoom slider

init(device: AVCaptureDevice, action: (CGFloat) -> Void)

Creates a slider to control the zoom level of the specified capture device with an action to respond to zoom changes.

