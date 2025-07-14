

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.Format
-  isStudioLightSupported 

Instance Property

# isStudioLightSupported

A Boolean value that indicates whether the format supports Studio Light.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 17.0+

``` source
var isStudioLightSupported: Bool { get }
```

## Discussion

See isStudioLightEnabled for more information on the Studio Light feature.

## See Also

### Determining Studio Light Support

var videoFrameRateRangeForStudioLight: AVFrameRateRange?

A value that indicates the minimum and maximum frame rates available when a user enables Studio Light.

