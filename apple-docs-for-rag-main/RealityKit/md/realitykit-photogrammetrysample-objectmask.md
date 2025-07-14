

- RealityKit
- PhotogrammetrySample
-  objectMask 

Instance Property

# objectMask

The image’s object mask.

iOS 17.0+iPadOS 17.0+Mac Catalyst 15.0+macOS 12.0+

``` source
var objectMask: CVPixelBuffer? { get set }
```

## Discussion

When a photograph of an object includes surrounding objects, such as plants, buildings, or people in an outdoor space, you can create an object mask to exclude the portions of the image that don’t contain the object. Masking extraneous image data reduces the number of landmarks RealityKit attempts to match, speeds up the object-creation process, and produces a more accurate 3D model.

Provide the object mask in kCVPixelFormatType_OneComponent8 format and with the same height and width as image. RealityKit ignores any pixel in image when the corresponding pixel in objectMask has a value of `0.0` (black) unless isObjectMaskingEnabled is set to `False` in the session’s configuration.

## See Also

### Describing the sample

let image: CVPixelBuffer

The image data for this sample.

var metadata: [String : Any]

An image’s EXIF metadata.

var depthDataMap: CVPixelBuffer?

The image’s depth data.

var gravity: CMAcceleration?

An image’s gravity vector.

