

- Image I/O
-  CGImageSourceCreateWithURL(\_:\_:) 

Function

# CGImageSourceCreateWithURL(\_:\_:)

Creates an image source that reads from a location specified by a URL.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CGImageSourceCreateWithURL(
    _ url: CFURL,
    _ options: CFDictionary?
) -> CGImageSource?
```

## Parameters 

`url`  

The URL of the image.

`options`  

A dictionary that specifies additional creation options. For a list of possible values, see Specifying the Read Options.

## Return Value

An image source. You’re responsible for releasing this type using CFRelease.

## See Also

### Creating an Image Source

func CGImageSourceCreateWithData(CFData, CFDictionary?) -> CGImageSource?

Creates an image source that reads from a Core Foundation data object.

func CGImageSourceCreateWithDataProvider(CGDataProvider, CFDictionary?) -> CGImageSource?

Creates an image source that reads data from the specified data provider.

func CGImageSourceCreateIncremental(CFDictionary?) -> CGImageSource

Creates an empty image source that you can use to accumulate incremental image data.

