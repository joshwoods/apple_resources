

- Image I/O
-  kCGImageAuxiliaryDataInfoData 

Global Variable

# kCGImageAuxiliaryDataInfoData

The auxiliary data for the image.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
let kCGImageAuxiliaryDataInfoData: CFString
```

## Discussion

The value of this property is a CFData. Use the kCGImagePropertyAuxiliaryDataType property to determine the format of this data.

## See Also

### Auxiliary Image Data

let kCGImagePropertyAuxiliaryData: CFString

An array of dictionaries that contain auxiliary data for the images.

let kCGImagePropertyAuxiliaryDataType: CFString

The type of the auxiliary data.

let kCGImageAuxiliaryDataInfoDataDescription: CFString

A dictionary of keys that describe the auxiliary data.

let kCGImageAuxiliaryDataInfoMetadata: CFString

The metadata for any auxiliary data.

