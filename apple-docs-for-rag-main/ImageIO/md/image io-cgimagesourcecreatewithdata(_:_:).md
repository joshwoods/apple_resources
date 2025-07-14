

- Image I/O
-  CGImageSourceCreateWithData(\_:\_:) 

Function

# CGImageSourceCreateWithData(\_:\_:)

Creates an image source that reads from a Core Foundation data object.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CGImageSourceCreateWithData(
    _ data: CFData,
    _ options: CFDictionary?
) -> CGImageSource?
```

## Parameters 

`data`  

The data object from which to read. For more information on data objects, see doc://com.apple.documentation/documentation/corefoundation/cfdata-rv9 (Swift), CFData (Objective-C), and Data Objects.

`options`  

A dictionary that specifies additional creation options. For a list of possible values, see Specifying the Read Options.

## Return Value

An image source. You’re responsible for releasing this type using CFRelease.

## See Also

### Creating an Image Source

func CGImageSourceCreateWithURL(CFURL, CFDictionary?) -> CGImageSource?

Creates an image source that reads from a location specified by a URL.

func CGImageSourceCreateWithDataProvider(CGDataProvider, CFDictionary?) -> CGImageSource?

Creates an image source that reads data from the specified data provider.

func CGImageSourceCreateIncremental(CFDictionary?) -> CGImageSource

Creates an empty image source that you can use to accumulate incremental image data.

