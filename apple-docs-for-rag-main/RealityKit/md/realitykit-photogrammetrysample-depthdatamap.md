

- RealityKit
- PhotogrammetrySample
-  depthDataMap 

Instance Property

# depthDataMap

The image’s depth data.

iOS 17.0+iPadOS 17.0+Mac Catalyst 15.0+macOS 12.0+

``` source
var depthDataMap: CVPixelBuffer? { get set }
```

## Discussion

Some cameras, including iPhone cameras, capture depth data in addition to image data. Providing this data can help PhotogrammetrySession determine the real-world scale of the photographed object and result in a correctly sized 3D object for placement in an AR scene. This property is read-only.

Depth data can be in either kCVPixelFormatType_DisparityFloat32 or kCVPixelFormatType_DepthFloat32 format.

## See Also

### Describing the sample

let image: CVPixelBuffer

The image data for this sample.

var metadata: [String : Any]

An image’s EXIF metadata.

var gravity: CMAcceleration?

An image’s gravity vector.

var objectMask: CVPixelBuffer?

The image’s object mask.

