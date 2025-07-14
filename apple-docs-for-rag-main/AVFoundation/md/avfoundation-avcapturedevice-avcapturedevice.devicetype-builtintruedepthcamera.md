

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.DeviceType
-  builtInTrueDepthCamera 

Type Property

# builtInTrueDepthCamera

A device that consists of two cameras, one Infrared and one YUV.

iOS 11.1+iPadOS 11.1+Mac Catalyst 14.0+tvOS 17.0+

``` source
static let builtInTrueDepthCamera: AVCaptureDevice.DeviceType
```

## Mentioned in 

Capturing Photos with Depth

## Discussion

The infrared camera provides high-quality depth information that’s synchronized and perspective corrected to the frame the YUV camera produces. While the resolution of the depth data and YUV frames may differ, their field of view and aspect ratio always match.

Important

To obtain a device of this type, use the default(_:for:position:) method or the AVCaptureDevice.DiscoverySession class. Other methods don’t discover devices of this type.

## See Also

### Depth Sensing

static let builtInLiDARDepthCamera: AVCaptureDevice.DeviceType

A device that consists of two cameras, one LiDAR and one YUV.

