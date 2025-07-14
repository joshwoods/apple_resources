

- AVFoundation
- AVPortraitEffectsMatte
-  pixelFormatType 

Instance Property

# pixelFormatType

The pixel format type of this portrait effects matte’s internal image.

iOS 12.0+iPadOS 12.0+Mac Catalyst 14.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
var pixelFormatType: OSType { get }
```

## Discussion

The only supported pixel format type for the matting image is kCVPixelFormatType_OneComponent8.

## See Also

### Examining a Portrait Effects Matte

Extracting Portrait Effects Matte Image Data from a Photo

Check for portrait effects matte metadata in existing images.

var mattingImage: CVPixelBuffer

The portrait effects matte’s internal image, formatted as a pixel buffer.

func dictionaryRepresentation(forAuxiliaryDataType: AutoreleasingUnsafeMutablePointer&lt;NSString?>?) -> [AnyHashable : Any]?

A dictionary of primitive map information used for writing an image file with a portrait effects matte.

