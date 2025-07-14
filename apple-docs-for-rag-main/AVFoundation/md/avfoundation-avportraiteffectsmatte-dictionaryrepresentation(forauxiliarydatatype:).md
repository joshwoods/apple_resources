

- AVFoundation
- AVPortraitEffectsMatte
-  dictionaryRepresentation(forAuxiliaryDataType:) 

Instance Method

# dictionaryRepresentation(forAuxiliaryDataType:)

A dictionary of primitive map information used for writing an image file with a portrait effects matte.

iOS 12.0+iPadOS 12.0+Mac Catalyst 14.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
func dictionaryRepresentation(forAuxiliaryDataType outAuxDataType: AutoreleasingUnsafeMutablePointer?) -> [AnyHashable : Any]?
```

## Parameters 

`outAuxDataType`  

Must be kCGImageAuxiliaryDataTypePortraitEffectsMatte.

## Return Value

A dictionary of primitive map information for CGImageDestinationAddAuxiliaryDataInfo(_:_:_:).

## See Also

### Examining a Portrait Effects Matte

Extracting Portrait Effects Matte Image Data from a Photo

Check for portrait effects matte metadata in existing images.

var mattingImage: CVPixelBuffer

The portrait effects matte’s internal image, formatted as a pixel buffer.

var pixelFormatType: OSType

The pixel format type of this portrait effects matte’s internal image.

