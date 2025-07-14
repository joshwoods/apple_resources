

- AVFoundation
- AVCapturePhotoOutput
-  isVirtualDeviceConstituentPhotoDeliveryEnabled 

Instance Property

# isVirtualDeviceConstituentPhotoDeliveryEnabled

A Boolean value that indicates whether the photo output delivers photos from constituent cameras of a virtual device.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var isVirtualDeviceConstituentPhotoDeliveryEnabled: Bool { get set }
```

## Discussion

You can only set this value to true when isVirtualDeviceConstituentPhotoDeliverySupported is true.

The default value is false.

Important

Virtual device constituent photo delivery requires a lengthy reconfiguration of the capture render pipeline, so enable this property prior to starting the capture session.

## See Also

### Configuring Virtual Device Capture

var isVirtualDeviceFusionSupported: Bool

A Boolean value that indicates whether the device supports virtual device image fusion.

var isVirtualDeviceConstituentPhotoDeliverySupported: Bool

A Boolean value that indicates whether the photo output configuration supports delivery of photos from constituent cameras of a virtual device.

