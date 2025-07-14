

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.Format
-  supportedMaxPhotoDimensions 

Instance Property

# supportedMaxPhotoDimensions

The maximum photo dimension this format supports.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 17.0+

``` source
@nonobjc
var supportedMaxPhotoDimensions: [CMVideoDimensions] { get }
```

## See Also

### Determining Photo Quality

var isHighPhotoQualitySupported: Bool

A Boolean value that indicates whether this format supports high-quality capture with the current quality prioritization setting.

var isHighestPhotoQualitySupported: Bool

A Boolean value that indicates whether this format supports the highest photo quality that the platform delivers.

