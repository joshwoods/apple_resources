

- Image I/O
-  kCGImageAuxiliaryDataInfoDataDescription 

Global Variable

# kCGImageAuxiliaryDataInfoDataDescription

A dictionary of keys that describe the auxiliary data.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
let kCGImageAuxiliaryDataInfoDataDescription: CFString
```

## Discussion

The value of this property is a CFDictionary. The keys in this dictionary may include kCGImagePropertyWidth, kCGImagePropertyHeight, and kCGImagePropertyBytesPerRow.

## See Also

### Auxiliary Image Data

let kCGImagePropertyAuxiliaryData: CFString

An array of dictionaries that contain auxiliary data for the images.

let kCGImagePropertyAuxiliaryDataType: CFString

The type of the auxiliary data.

let kCGImageAuxiliaryDataInfoData: CFString

The auxiliary data for the image.

let kCGImageAuxiliaryDataInfoMetadata: CFString

The metadata for any auxiliary data.

