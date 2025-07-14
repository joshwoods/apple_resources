

- Image I/O
- Image Properties
-  Individual Image Properties 

API Collection

# Individual Image Properties

Properties that apply to an individual image in an image source.

## Overview

Access these properties using the CGImageSourceCopyPropertiesAtIndex(_:_:_:) or CGImageSourceCopyAuxiliaryDataInfoAtIndex(_:_:_:) function.

## Topics

### Image Size

let kCGImagePropertyHeight: CFString

The height of the image, in the image’s coordinate space.

let kCGImagePropertyWidth: CFString

The width of the image, in the image’s coordinate space.

let kCGImagePropertyBytesPerRow: CFString

The total number of bytes in each row of the image.

### Auxiliary Data Types

let kCGImageAuxiliaryDataTypeDepth: CFString

The type for depth map information.

let kCGImageAuxiliaryDataTypeDisparity: CFString

The type for image disparity information.

let kCGImageAuxiliaryDataTypeHDRGainMap: CFString

The type for High Dynamic Range (HDR) gain map information.

let kCGImageAuxiliaryDataTypePortraitEffectsMatte: CFString

The type for portrait effects matte information.

let kCGImageAuxiliaryDataTypeSemanticSegmentationGlassesMatte: CFString

The type for glasses matte informaton.

let kCGImageAuxiliaryDataTypeSemanticSegmentationHairMatte: CFString

The type for hair matte information.

let kCGImageAuxiliaryDataTypeSemanticSegmentationSkinMatte: CFString

The type for skin matte informaton.

let kCGImageAuxiliaryDataTypeSemanticSegmentationSkyMatte: CFString

The type for sky matte information.

let kCGImageAuxiliaryDataTypeSemanticSegmentationTeethMatte: CFString

The type for teeth matte information.

### Auxiliary Image Data

let kCGImagePropertyAuxiliaryData: CFString

An array of dictionaries that contain auxiliary data for the images.

let kCGImagePropertyAuxiliaryDataType: CFString

The type of the auxiliary data.

let kCGImageAuxiliaryDataInfoData: CFString

The auxiliary data for the image.

let kCGImageAuxiliaryDataInfoDataDescription: CFString

A dictionary of keys that describe the auxiliary data.

let kCGImageAuxiliaryDataInfoMetadata: CFString

The metadata for any auxiliary data.

### Open EXR Properties

let kCGImagePropertyOpenEXRDictionary: CFString

A dictionary of properties specific to the OpenEXR metadata standard.

let kCGImagePropertyOpenEXRAspectRatio: CFString

The aspect ratio of the image.

## See Also

### Image Information

let kCGImagePropertyImageCount: CFString

The number of images in the file.

let kCGImagePropertyIsIndexed: CFString

A Boolean value that indicates whether the image contains indexed pixel samples.

let kCGImagePropertyImages: CFString

An array of dictionaries, each of which contains metadata for one of the images in the file.

let kCGImagePropertyThumbnailImages: CFString

let kCGImagePropertyPrimaryImage: CFString

The index of the primary image in the file.

let kCGImagePropertyIsFloat: CFString

A Boolean value that indicates whether the image contains floating-point pixel samples.

let kCGImagePropertyOrientation: CFString

The intended display orientation of the image.

enum CGImagePropertyOrientation

A value describing the intended display orientation for an image.

