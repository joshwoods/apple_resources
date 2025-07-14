

- AVFoundation
- AVPortraitEffectsMatte
-  mattingImage 

Instance Property

# mattingImage

The portrait effects matte’s internal image, formatted as a pixel buffer.

iOS 12.0+iPadOS 12.0+Mac Catalyst 14.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
var mattingImage: CVPixelBuffer { get }
```

## Discussion

Query the pixel format using the pixelFormatType property.

## See Also

### Examining a Portrait Effects Matte

Extracting Portrait Effects Matte Image Data from a Photo

Check for portrait effects matte metadata in existing images.

var pixelFormatType: OSType

The pixel format type of this portrait effects matte’s internal image.

func dictionaryRepresentation(forAuxiliaryDataType: AutoreleasingUnsafeMutablePointer&lt;NSString?>?) -> [AnyHashable : Any]?

A dictionary of primitive map information used for writing an image file with a portrait effects matte.

