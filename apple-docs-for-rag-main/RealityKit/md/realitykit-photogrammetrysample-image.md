

- RealityKit
- PhotogrammetrySample
-  image 

Instance Property

# image

The image data for this sample.

iOS 17.0+iPadOS 17.0+Mac Catalyst 15.0+macOS 12.0+

``` source
let image: CVPixelBuffer
```

## Discussion

Provide image data in the kCVPixelFormatType_32BGRA or kCVPixelFormatType_32ARGB pixel formats.

## See Also

### Describing the sample

var metadata: [String : Any]

An image’s EXIF metadata.

var depthDataMap: CVPixelBuffer?

The image’s depth data.

var gravity: CMAcceleration?

An image’s gravity vector.

var objectMask: CVPixelBuffer?

The image’s object mask.

