

- AVFoundation
- AVSemanticSegmentationMatte
-  pixelFormatType 

Instance Property

# pixelFormatType

The pixel format type for this object’s internal matting image.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var pixelFormatType: OSType { get }
```

## Discussion

Currently, the only supported pixel format type for the matting image is kCVPixelFormatType_OneComponent8.

## See Also

### Inspecting a Segmentation Matte

var matteType: AVSemanticSegmentationMatte.MatteType

The semantic segmentation matte image type.

struct MatteType

A structure that defines the types of segmentation matte images that you can capture along with the primary image.

var mattingImage: CVPixelBuffer

The semantic segmentation matte’s internal image.

