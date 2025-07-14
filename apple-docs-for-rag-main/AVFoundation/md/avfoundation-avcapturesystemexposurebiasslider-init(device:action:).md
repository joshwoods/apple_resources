

- AVFoundation
- AVCaptureSystemExposureBiasSlider
-  init(device:action:) 

Initializer

# init(device:action:)

Creates a slider to control the exposure bias of the specified capture device with an action to respond to exposure bias changes.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+

``` source
init(
    device: AVCaptureDevice,
    action: @escaping @MainActor (Float) -> Void
)
```

## Parameters 

`device`  

The capture device to control.

`action`  

An action the system calls on the main actor to handle changes to the device’s exposureTargetBias property.

## Discussion

The system only calls the specified action when the exposure bias slider changes the device’s videoZoomFactor property value. If you need to react to other sources of changes to the exposure target bias, use key-value observation instead.

Important

Don’t change the capture device’s exposure target bias when the system calls the action.

## See Also

### Creating an exposure bias slider

init(device: AVCaptureDevice)

Creates a slider to control the exposure bias of the specified capture device.

