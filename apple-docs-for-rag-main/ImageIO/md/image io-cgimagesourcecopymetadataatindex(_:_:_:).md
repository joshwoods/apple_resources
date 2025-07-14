

- Image I/O
-  CGImageSourceCopyMetadataAtIndex(\_:\_:\_:) 

Function

# CGImageSourceCopyMetadataAtIndex(\_:\_:\_:)

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CGImageSourceCopyMetadataAtIndex(
    _ isrc: CGImageSource,
    _ index: Int,
    _ options: CFDictionary?
) -> CGImageMetadata?
```

## See Also

### Functions

func CGImageDestinationAddImageAndMetadata(CGImageDestination, CGImage, CGImageMetadata?, CFDictionary?)

func CGImageDestinationCopyImageSource(CGImageDestination, CGImageSource, CFDictionary?, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> Bool

func CGImageSourceRemoveCacheAtIndex(CGImageSource, Int)

func CGImageSourceSetAllowableTypes(CFArray) -> OSStatus

