

- Image I/O
-  CGImageDestinationAddImageFromSource(\_:\_:\_:\_:) 

Function

# CGImageDestinationAddImageFromSource(\_:\_:\_:\_:)

Adds an image from an image source to an image destination.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CGImageDestinationAddImageFromSource(
    _ idst: CGImageDestination,
    _ isrc: CGImageSource,
    _ index: Int,
    _ properties: CFDictionary?
)
```

## Parameters 

`idst`  

The image destination to modify.

`isrc`  

An image source that contains the image.

`index`  

The index of the image in the image source. Specify a valid, zero-based index into the images of the image source. If the index is invalid, this method returns `NULL`.

`properties`  

An optional dictionary that specifies additional image property information. The added image automatically inherits the properties found in the image source. Use this dictionary to add properties to the image, or to modify one of the inherited properties. To remove an inherited property altogether, specify `NULL` for the property’s value. For a list of possible values, see Image Properties and Configuring the Image Behaviors.

## See Also

### Adding Images to the Destination

func CGImageDestinationAddImage(CGImageDestination, CGImage, CFDictionary?)

Adds an image to an image destination.

