

- AVFoundation
- AVCaptureSession
-  isMultitaskingCameraAccessSupported 

Instance Property

# isMultitaskingCameraAccessSupported

A Boolean value that indicates whether the capture session supports using the camera while multitasking.

iOS 16.0+iPadOS 16.0+tvOS 17.0+

``` source
var isMultitaskingCameraAccessSupported: Bool { get }
```

## Discussion

Query this property to determine whether you can use the camera while multitasking by setting the state of the isMultitaskingCameraAccessEnabled property to true.

Prior to iOS 18, this property is true on iPads that support Stage Manager with an extended display. In apps linked against iOS 18 or later, this property is true for video conferencing apps (those that use `voip` as one of their UIBackgroundModes). This property also returns true for iOS applications that have the com.apple.developer.avfoundation.multitasking-camera-access entitlement.

In tvOS, this property is always true.

Note

This property is key-value observable. If the value changes from true to false, the value of isMultitaskingCameraAccessEnabled also changes to false.

To learn about best practices for using the camera while multitasking, see Accessing the camera while multitasking on iPad.

## See Also

### Configuring Multitasking

var isMultitaskingCameraAccessEnabled: Bool

A Boolean value that indicates whether the capture session enables access to the camera while multitasking.

