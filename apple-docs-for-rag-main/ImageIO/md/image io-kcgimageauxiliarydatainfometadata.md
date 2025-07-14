

- Image I/O
-  kCGImageAuxiliaryDataInfoMetadata 

Global Variable

# kCGImageAuxiliaryDataInfoMetadata

The metadata for any auxiliary data.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
let kCGImageAuxiliaryDataInfoMetadata: CFString
```

## Discussion

The value of this property is a CGImageMetadata type. Use it to obtain any metadata associated with the auxiliary data.

## See Also

### Auxiliary Image Data

let kCGImagePropertyAuxiliaryData: CFString

An array of dictionaries that contain auxiliary data for the images.

let kCGImagePropertyAuxiliaryDataType: CFString

The type of the auxiliary data.

let kCGImageAuxiliaryDataInfoData: CFString

The auxiliary data for the image.

let kCGImageAuxiliaryDataInfoDataDescription: CFString

A dictionary of keys that describe the auxiliary data.

