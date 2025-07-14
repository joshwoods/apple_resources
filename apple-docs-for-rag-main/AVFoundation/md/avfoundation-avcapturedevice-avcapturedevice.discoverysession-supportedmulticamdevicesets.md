

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.DiscoverySession
-  supportedMultiCamDeviceSets 

Instance Property

# supportedMultiCamDeviceSets

Sets of capture devices that you can use simultaneously in a multi-camera session.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 2.1+

``` source
var supportedMultiCamDeviceSets: [Set] { get }
```

## Discussion

You may use multiple cameras as device inputs to an AVCaptureMultiCamSession, as long as one of the supported multi-camera device sets includes the device.

## See Also

### Finding Devices

var devices: [AVCaptureDevice]

A list of devices that match the search criteria of the discovery session.

