

- Core Video
-  CVPixelFormatDescriptionArrayCreateWithAllPixelFormatTypes(\_:) 

Function

# CVPixelFormatDescriptionArrayCreateWithAllPixelFormatTypes(\_:)

Returns all the pixel format descriptions known to Core Video.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CVPixelFormatDescriptionArrayCreateWithAllPixelFormatTypes(_ allocator: CFAllocator?) -> CFArray?
```

## Parameters 

`allocator`  

The allocator to use when creating the description. Pass `NULL` to specify the default allocator.

## Return Value

An array of Core Foundation dictionaries, each containing a pixel format description. See Pixel Format Description Keys for a list of keys relevant to the format description.

