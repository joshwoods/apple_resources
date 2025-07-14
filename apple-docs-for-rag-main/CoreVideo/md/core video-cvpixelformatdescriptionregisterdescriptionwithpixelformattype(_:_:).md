

- Core Video
-  CVPixelFormatDescriptionRegisterDescriptionWithPixelFormatType(\_:\_:) 

Function

# CVPixelFormatDescriptionRegisterDescriptionWithPixelFormatType(\_:\_:)

Registers a pixel format description with Core Video.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CVPixelFormatDescriptionRegisterDescriptionWithPixelFormatType(
    _ description: CFDictionary,
    _ pixelFormat: OSType
)
```

## Parameters 

`description`  

A Core Foundation dictionary containing the pixel format description. See Pixel Format Description Keys for a list of required and optional keys.

`pixelFormat`  

The four-character code (type `OSType`) identifier for this pixel format.

## Discussion

If you are using a custom pixel format, you must register the format with Core Video using this function. See Technical Q&amp;A 1401: Registering Custom Pixel Formats with QuickTime and Core Video for more details.

## See Also

### Related Documentation

Core Video Programming Guide

### Creating Format Descriptions

func CVPixelFormatDescriptionCreateWithPixelFormatType(CFAllocator?, OSType) -> CFDictionary?

Creates a pixel format description from a given `OSType` identifier.

