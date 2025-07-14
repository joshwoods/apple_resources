

- AVFoundation
- AVCaptureSystemZoomSlider
-  init(device:action:) 

Initializer

# init(device:action:)

Creates a slider to control the zoom level of the specified capture device with an action to respond to zoom changes.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+

``` source
init(
    device: AVCaptureDevice,
    action: @escaping @MainActor (CGFloat) -> Void
)
```

## Parameters 

`device`  

The capture device to control.

`action`  

An action the system calls on the main actor to respond to changes to the device’s videoZoomFactor property.

## Discussion

The system calls the specified action only when the zoom slider changes the device’s videoZoomFactor property value. If your app needs to react to other sources of video zoom factor changes like ramp(toVideoZoomFactor:withRate:), use key-value observation instead.

Important

Don’t change the capture device’s video zoom factor when the system calls the action.

## See Also

### Creating a zoom slider

init(device: AVCaptureDevice)

Creates a slider to control the video zoom factor of a capture device.

