

- AVFoundation
- AVCapturePhotoOutput
-  isVirtualDeviceConstituentPhotoDeliverySupported 

Instance Property

# isVirtualDeviceConstituentPhotoDeliverySupported

A Boolean value that indicates whether the photo output configuration supports delivery of photos from constituent cameras of a virtual device.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var isVirtualDeviceConstituentPhotoDeliverySupported: Bool { get }
```

## Discussion

The system only supports virtual device constituent photo delivery for certain capture session presets and capture device formats.

When switching cameras or formats, this property may change. When this property changes from true to false, isVirtualDeviceConstituentPhotoDeliveryEnabled also reverts to false.

This property is key-value observable.

## See Also

### Configuring Virtual Device Capture

var isVirtualDeviceFusionSupported: Bool

A Boolean value that indicates whether the device supports virtual device image fusion.

var isVirtualDeviceConstituentPhotoDeliveryEnabled: Bool

A Boolean value that indicates whether the photo output delivers photos from constituent cameras of a virtual device.

