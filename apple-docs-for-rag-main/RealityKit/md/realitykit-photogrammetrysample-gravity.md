

- RealityKit
- PhotogrammetrySample
-  gravity 

Instance Property

# gravity

An image’s gravity vector.

iOS 17.0+iPadOS 17.0+Mac Catalyst 15.0+macOS 12.0+

``` source
var gravity: CMAcceleration? { get set }
```

## Discussion

Some cameras, including iPhone cameras, capture a gravity vector for each image. This vector indicates the orientation of the camera at the moment you took the picture. RealityKit uses this gravity vector to improve landmark matching with the other images in the session.

## See Also

### Describing the sample

let image: CVPixelBuffer

The image data for this sample.

var metadata: [String : Any]

An image’s EXIF metadata.

var depthDataMap: CVPixelBuffer?

The image’s depth data.

var objectMask: CVPixelBuffer?

The image’s object mask.

