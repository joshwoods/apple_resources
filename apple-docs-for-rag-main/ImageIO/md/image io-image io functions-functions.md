

- Image I/O
-  Image I/O Functions 

API Collection

# Image I/O Functions

## Topics

### Functions

func CGImageDestinationAddImageAndMetadata(CGImageDestination, CGImage, CGImageMetadata?, CFDictionary?)

func CGImageDestinationCopyImageSource(CGImageDestination, CGImageSource, CFDictionary?, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> Bool

func CGImageSourceCopyMetadataAtIndex(CGImageSource, Int, CFDictionary?) -> CGImageMetadata?

func CGImageSourceRemoveCacheAtIndex(CGImageSource, Int)

func CGImageSourceSetAllowableTypes(CFArray) -> OSStatus

## See Also

### Reference

Image I/O Constants

Image I/O Macros

