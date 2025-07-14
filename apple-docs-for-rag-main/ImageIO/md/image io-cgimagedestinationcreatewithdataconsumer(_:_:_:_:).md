

- Image I/O
-  CGImageDestinationCreateWithDataConsumer(\_:\_:\_:\_:) 

Function

# CGImageDestinationCreateWithDataConsumer(\_:\_:\_:\_:)

Creates an image destination that writes to the specified data consumer.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CGImageDestinationCreateWithDataConsumer(
    _ consumer: CGDataConsumer,
    _ type: CFString,
    _ count: Int,
    _ options: CFDictionary?
) -> CGImageDestination?
```

## Parameters 

`consumer`  

A data consumer object to store the image data.

`type`  

The uniform type identifier of the resulting image file. For a list of system-declared and third-party identifiers, see Uniform Type Identifiers.

`count`  

The number of images (not including thumbnail images) you want to include in the image file.

`options`  

Future options. Specify `NULL` for this parameter.

## Return Value

An image destination, or `NULL` if an error occurs. You are responsible for releasing this object using CFRelease.

## See Also

### Creating an Image Destination

func CGImageDestinationCreateWithURL(CFURL, CFString, Int, CFDictionary?) -> CGImageDestination?

Creates an image destination that writes image data to the specified URL.

func CGImageDestinationCreateWithData(CFMutableData, CFString, Int, CFDictionary?) -> CGImageDestination?

Creates an image destination that writes to a Core Foundation mutable data object.

