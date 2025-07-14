

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.DiscoverySession
-  init(deviceTypes:mediaType:position:) 

Initializer

# init(deviceTypes:mediaType:position:)

Creates a discovery session that finds devices that match the specified criteria.

iOS 10.0+iPadOS 10.0+Mac Catalyst 14.0+macOS 10.15+tvOS 17.0+visionOS 2.1+

``` source
convenience init(
    deviceTypes: [AVCaptureDevice.DeviceType],
    mediaType: AVMediaType?,
    position: AVCaptureDevice.Position
)
```

## Parameters 

`deviceTypes`  

A list of device types to search for, such as builtInWideAngleCamera and builtInMicrophone. The array must contain at least one valid AVCaptureDevice.DeviceType value.

`mediaType`  

The media type to capture, such as video or audio. Pass `nil` to search for devices regardless of supported media types.

`position`  

The position of capture device to search for, relative to system hardware (front- or back-facing). Pass AVCaptureDevice.Position.unspecified to search for devices regardless of position.

## Return Value

A new discovery session.

## Discussion

After creating a discovery session, query its devices property to examine matching devices and choose one for capture.

