

- Image I/O
-  CGImageSourceCreateIncremental(\_:) 

Function

# CGImageSourceCreateIncremental(\_:)

Creates an empty image source that you can use to accumulate incremental image data.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CGImageSourceCreateIncremental(_ options: CFDictionary?) -> CGImageSource
```

## Parameters 

`options`  

A dictionary that specifies additional creation options. For a list of possible values, see Specifying the Read Options.

## Return Value

An empty image source object. You’re responsible for releasing this type using CFRelease.

## Discussion

This function creates an empty image source container, which you use to accumulate data downloaded in chunks from the network. To add new chunks of data to the image source, call the CGImageSourceUpdateDataProvider(_:_:_:) or CGImageSourceUpdateData(_:_:_:) functions.

## See Also

### Creating an Image Source

func CGImageSourceCreateWithURL(CFURL, CFDictionary?) -> CGImageSource?

Creates an image source that reads from a location specified by a URL.

func CGImageSourceCreateWithData(CFData, CFDictionary?) -> CGImageSource?

Creates an image source that reads from a Core Foundation data object.

func CGImageSourceCreateWithDataProvider(CGDataProvider, CFDictionary?) -> CGImageSource?

Creates an image source that reads data from the specified data provider.

