

- Image I/O
-  CGImageDestinationAddAuxiliaryDataInfo(\_:\_:\_:) 

Function

# CGImageDestinationAddAuxiliaryDataInfo(\_:\_:\_:)

Sets the auxiliary data, such as mattes and depth information, that accompany the image.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func CGImageDestinationAddAuxiliaryDataInfo(
    _ idst: CGImageDestination,
    _ auxiliaryImageDataType: CFString,
    _ auxiliaryDataInfoDictionary: CFDictionary
)
```

## Parameters 

`idst`  

The image destination to modify.

`auxiliaryImageDataType`  

The type of auxiliary information you want to add. For a list of possible values, see Auxiliary Data Types.

`auxiliaryDataInfoDictionary`  

A dictionary that contains the kCGImageAuxiliaryDataInfoData, kCGImageAuxiliaryDataInfoDataDescription, and kCGImageAuxiliaryDataInfoMetadata keys. Use those keys to describe the depth or matte information.

## Discussion

Call this method after you add an image to the image destination. This method adds the specified depth or matte information to the most recently added image.

## See Also

### Adding Metadata to the Image

func CGImageDestinationSetProperties(CGImageDestination, CFDictionary?)

Applies one or more properties to all images in an image destination.

