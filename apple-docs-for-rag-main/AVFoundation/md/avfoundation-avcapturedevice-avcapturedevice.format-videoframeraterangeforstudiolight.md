

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.Format
-  videoFrameRateRangeForStudioLight 

Instance Property

# videoFrameRateRangeForStudioLight

A value that indicates the minimum and maximum frame rates available when a user enables Studio Light.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 17.0+

``` source
var videoFrameRateRangeForStudioLight: AVFrameRateRange? { get }
```

## Discussion

Devices may support a limited frame rate range when Studio Light is active. If the format doesn’t support Studio Light, this property is `nil`.

## See Also

### Determining Studio Light Support

var isStudioLightSupported: Bool

A Boolean value that indicates whether the format supports Studio Light.

