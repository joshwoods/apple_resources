

- Image I/O
-  CGImageDestinationCopyImageSource(\_:\_:\_:\_:) 

Function

# CGImageDestinationCopyImageSource(\_:\_:\_:\_:)

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CGImageDestinationCopyImageSource(
    _ idst: CGImageDestination,
    _ isrc: CGImageSource,
    _ options: CFDictionary?,
    _ err: UnsafeMutablePointer?>?
) -> Bool
```

## See Also

### Functions

func CGImageDestinationAddImageAndMetadata(CGImageDestination, CGImage, CGImageMetadata?, CFDictionary?)

func CGImageSourceCopyMetadataAtIndex(CGImageSource, Int, CFDictionary?) -> CGImageMetadata?

func CGImageSourceRemoveCacheAtIndex(CGImageSource, Int)

func CGImageSourceSetAllowableTypes(CFArray) -> OSStatus

