

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.DeviceType
-  builtInLiDARDepthCamera 

Type Property

# builtInLiDARDepthCamera

A device that consists of two cameras, one LiDAR and one YUV.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+tvOS 17.0+

``` source
static let builtInLiDARDepthCamera: AVCaptureDevice.DeviceType
```

## Discussion

The LiDAR camera provides high-quality, high-accuracy depth information by measuring the round trip of an artificial light signal that a laser emits. The device synchronizes and perspective-corrects this data to frames that the YUV camera produces. While the resolution of the depth data and YUV frames may differ, their field of view and aspect ratio always match.

Note

You can only discover devices of this type by using an AVCaptureDevice.DiscoverySession or by calling the default(_:for:position:) method.

## See Also

### Depth Sensing

static let builtInTrueDepthCamera: AVCaptureDevice.DeviceType

A device that consists of two cameras, one Infrared and one YUV.

