

- Image I/O
-  kCGImagePropertyAuxiliaryData 

Global Variable

# kCGImagePropertyAuxiliaryData

An array of dictionaries that contain auxiliary data for the images.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
let kCGImagePropertyAuxiliaryData: CFString
```

## Discussion

The value of this key is a CFArray. Each CFDictionary in the array contains auxiliary data for one of the images in the file. Use the kCGImagePropertyAuxiliaryDataType key to determine the type of data associated with the image.

## See Also

### Auxiliary Image Data

let kCGImagePropertyAuxiliaryDataType: CFString

The type of the auxiliary data.

let kCGImageAuxiliaryDataInfoData: CFString

The auxiliary data for the image.

let kCGImageAuxiliaryDataInfoDataDescription: CFString

A dictionary of keys that describe the auxiliary data.

let kCGImageAuxiliaryDataInfoMetadata: CFString

The metadata for any auxiliary data.

