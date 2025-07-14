

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.DiscoverySession
-  devices 

Instance Property

# devices

A list of devices that match the search criteria of the discovery session.

iOS 10.0+iPadOS 10.0+Mac Catalyst 14.0+macOS 10.15+tvOS 17.0+visionOS 2.1+

``` source
var devices: [AVCaptureDevice] { get }
```

## Mentioned in 

Choosing a Capture Device

## Discussion

Querying this property provides an array devices currently available on the system. The system sorts the device list according to the order you specified when you created the discovery session. If you created the session with a position of AVCaptureDevice.Position.unspecified, the system further sorts them by position in the AVCaptureDevice.Position enumeration.

Key-value observe this property to monitor changes to the device list.

## See Also

### Finding Devices

var supportedMultiCamDeviceSets: [Set&lt;AVCaptureDevice>]

Sets of capture devices that you can use simultaneously in a multi-camera session.

