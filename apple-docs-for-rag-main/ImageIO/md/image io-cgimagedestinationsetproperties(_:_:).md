

- Image I/O
-  CGImageDestinationSetProperties(\_:\_:) 

Function

# CGImageDestinationSetProperties(\_:\_:)

Applies one or more properties to all images in an image destination.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CGImageDestinationSetProperties(
    _ idst: CGImageDestination,
    _ properties: CFDictionary?
)
```

## Parameters 

`idst`  

The image destination to modify

`properties`  

A dictionary that contains the properties to apply. For a list of possible values, see Image Properties and Configuring the Image Behaviors.

## See Also

### Adding Metadata to the Image

func CGImageDestinationAddAuxiliaryDataInfo(CGImageDestination, CFString, CFDictionary)

Sets the auxiliary data, such as mattes and depth information, that accompany the image.

