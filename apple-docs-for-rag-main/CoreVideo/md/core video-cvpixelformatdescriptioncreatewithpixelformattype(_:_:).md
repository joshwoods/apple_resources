

- Core Video
-  CVPixelFormatDescriptionCreateWithPixelFormatType(\_:\_:) 

Function

# CVPixelFormatDescriptionCreateWithPixelFormatType(\_:\_:)

Creates a pixel format description from a given `OSType` identifier.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CVPixelFormatDescriptionCreateWithPixelFormatType(
    _ allocator: CFAllocator?,
    _ pixelFormat: OSType
) -> CFDictionary?
```

## Parameters 

`allocator`  

The allocator to use when creating the description. Pass `NULL` to specify the default allocator.

`pixelFormat`  

A four-character code that identifies the pixel format you want to obtain.

## Return Value

A Core Foundation dictionary containing the pixel format description. See Pixel Format Description Keys for a list of keys relevant to the format description.

## See Also

### Creating Format Descriptions

func CVPixelFormatDescriptionRegisterDescriptionWithPixelFormatType(CFDictionary, OSType)

Registers a pixel format description with Core Video.

