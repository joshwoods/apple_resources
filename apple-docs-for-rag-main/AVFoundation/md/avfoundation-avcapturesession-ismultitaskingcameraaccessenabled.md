

- AVFoundation
- AVCaptureSession
-  isMultitaskingCameraAccessEnabled 

Instance Property

# isMultitaskingCameraAccessEnabled

A Boolean value that indicates whether the capture session enables access to the camera while multitasking.

iOS 16.0+iPadOS 16.0+tvOS 17.0+

``` source
var isMultitaskingCameraAccessEnabled: Bool { get set }
```

## Discussion

The default value is false.

Important

For apps that have the com.apple.developer.avfoundation.multitasking-camera-access entitlement, this property value defaults to true if isMultitaskingCameraAccessSupported is also true.

If the value of the isMultitaskingCameraAccessSupported property is true, you can enable multitasking camera access by setting this value to true prior to starting the capture session.

This property is key-value observable.

Note

If you enable multitasking camera access, the system doesn’t interrupt the capture session with a reason of AVCaptureSession.InterruptionReason.videoDeviceNotAvailableWithMultipleForegroundApps.

To learn about best practices for using the camera while multitasking, see Accessing the camera while multitasking on iPad.

## See Also

### Configuring Multitasking

var isMultitaskingCameraAccessSupported: Bool

A Boolean value that indicates whether the capture session supports using the camera while multitasking.

