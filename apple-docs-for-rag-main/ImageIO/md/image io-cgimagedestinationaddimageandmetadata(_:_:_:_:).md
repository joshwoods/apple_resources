

- Image I/O
-  CGImageDestinationAddImageAndMetadata(\_:\_:\_:\_:) 

Function

# CGImageDestinationAddImageAndMetadata(\_:\_:\_:\_:)

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CGImageDestinationAddImageAndMetadata(
    _ idst: CGImageDestination,
    _ image: CGImage,
    _ metadata: CGImageMetadata?,
    _ options: CFDictionary?
)
```

## See Also

### Functions

func CGImageDestinationCopyImageSource(CGImageDestination, CGImageSource, CFDictionary?, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> Bool

func CGImageSourceCopyMetadataAtIndex(CGImageSource, Int, CFDictionary?) -> CGImageMetadata?

func CGImageSourceRemoveCacheAtIndex(CGImageSource, Int)

func CGImageSourceSetAllowableTypes(CFArray) -> OSStatus

