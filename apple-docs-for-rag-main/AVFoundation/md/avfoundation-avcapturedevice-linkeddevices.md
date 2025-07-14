

- AVFoundation
- AVCaptureDevice
-  linkedDevices 

Instance Property

# linkedDevices

An array of capture devices that are physically linked to a device.

macOS 10.7+

``` source
var linkedDevices: [AVCaptureDevice] { get }
```

## Discussion

For an external iSight camera, the array contains an AVCaptureDevice instance that represents the external iSight microphone.

