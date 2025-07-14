

- Image I/O
-  kCGImagePropertyAuxiliaryDataType 

Global Variable

# kCGImagePropertyAuxiliaryDataType

The type of the auxiliary data.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
let kCGImagePropertyAuxiliaryDataType: CFString
```

## Discussion

The value of this property is a CFString. The value of this key might be kCGImageAuxiliaryDataTypeDisparity, kCGImageAuxiliaryDataTypeDepth, or another auxiliary data type.

## See Also

### Auxiliary Image Data

let kCGImagePropertyAuxiliaryData: CFString

An array of dictionaries that contain auxiliary data for the images.

let kCGImageAuxiliaryDataInfoData: CFString

The auxiliary data for the image.

let kCGImageAuxiliaryDataInfoDataDescription: CFString

A dictionary of keys that describe the auxiliary data.

let kCGImageAuxiliaryDataInfoMetadata: CFString

The metadata for any auxiliary data.

