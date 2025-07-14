

- AVFoundation
- AVSemanticSegmentationMatte
-  matteType 

Instance Property

# matteType

The semantic segmentation matte image type.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var matteType: AVSemanticSegmentationMatte.MatteType { get }
```

## Discussion

A semantic segmentation matte’s matteType is immutable for the life of the object.

## See Also

### Inspecting a Segmentation Matte

struct MatteType

A structure that defines the types of segmentation matte images that you can capture along with the primary image.

var mattingImage: CVPixelBuffer

The semantic segmentation matte’s internal image.

var pixelFormatType: OSType

The pixel format type for this object’s internal matting image.

