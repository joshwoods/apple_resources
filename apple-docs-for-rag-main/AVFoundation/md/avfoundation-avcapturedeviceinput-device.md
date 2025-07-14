

- AVFoundation
- AVCaptureDeviceInput
-  device 

Instance Property

# device

A capture device associated with this input.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+visionOS 1.0+

``` source
var device: AVCaptureDevice { get }
```

## See Also

### Accessing the Device

func ports(for: AVMediaType?, sourceDeviceType: AVCaptureDevice.DeviceType?, sourceDevicePosition: AVCaptureDevice.Position) -> [AVCaptureInput.Port]

Retrieves a virtual device’s constituent device ports for use in a multi-camera session.

