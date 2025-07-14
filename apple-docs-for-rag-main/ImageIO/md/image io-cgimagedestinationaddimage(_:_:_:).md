

- Image I/O
-  CGImageDestinationAddImage(\_:\_:\_:) 

Function

# CGImageDestinationAddImage(\_:\_:\_:)

Adds an image to an image destination.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CGImageDestinationAddImage(
    _ idst: CGImageDestination,
    _ image: CGImage,
    _ properties: CFDictionary?
)
```

## Parameters 

`idst`  

The image destination to modify.

`image`  

The image to add.

`properties`  

An optional dictionary that specifies the properties of the added image. Specify `NULL` to omit any additional properties. For a list of possible values, see Image Properties and Configuring the Image Behaviors.

## Discussion

The function logs an error if you add more images than what you specified when you created the image destination.

## See Also

### Adding Images to the Destination

func CGImageDestinationAddImageFromSource(CGImageDestination, CGImageSource, Int, CFDictionary?)

Adds an image from an image source to an image destination.

