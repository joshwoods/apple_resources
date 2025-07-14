

- AVFoundation
- AVSemanticSegmentationMatte
-  mattingImage 

Instance Property

# mattingImage

The semantic segmentation matte’s internal image.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var mattingImage: CVPixelBuffer { get }
```

## Discussion

You can determine the pixel buffer’s format type using the pixelFormatType property.

## See Also

### Inspecting a Segmentation Matte

var matteType: AVSemanticSegmentationMatte.MatteType

The semantic segmentation matte image type.

struct MatteType

A structure that defines the types of segmentation matte images that you can capture along with the primary image.

var pixelFormatType: OSType

The pixel format type for this object’s internal matting image.

