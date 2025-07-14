

- AVFoundation
- AVCaptureSystemExposureBiasSlider
-  init(device:) 

Initializer

# init(device:)

Creates a slider to control the exposure bias of the specified capture device.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+

``` source
init(device: AVCaptureDevice)
```

## Parameters 

`device`  

The capture device to control.

## Discussion

You can only create an exposure bias slider with a device that support’s setting its exposureTargetBias property value.

## See Also

### Creating an exposure bias slider

init(device: AVCaptureDevice, action: (Float) -> Void)

Creates a slider to control the exposure bias of the specified capture device with an action to respond to exposure bias changes.

