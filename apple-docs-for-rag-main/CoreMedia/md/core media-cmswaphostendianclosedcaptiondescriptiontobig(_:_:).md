

- Core Media
-  CMSwapHostEndianClosedCaptionDescriptionToBig(\_:\_:) 

Function

# CMSwapHostEndianClosedCaptionDescriptionToBig(\_:\_:)

Converts a closed caption description structure from host-endian to big-endian, in place.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMSwapHostEndianClosedCaptionDescriptionToBig(
    _ closedCaptionDescriptionData: UnsafeMutablePointer,
    _ closedCaptionDescriptionSize: Int
) -> OSStatus
```

## Parameters 

`closedCaptionDescriptionData`  

ClosedCaptionDescription data structure in host-endian byte ordering to be converted to big-endian byte ordering.

`closedCaptionDescriptionSize`  

Size of ClosedCaptionDescription data structure.

## See Also

### Working with Closed Captioning Descriptions

struct CMClosedCaptionDescriptionFlavor

Types that represent closed caption format descriptions.

func CMClosedCaptionFormatDescriptionCopyAsBigEndianClosedCaptionDescriptionBlockBuffer(allocator: CFAllocator?, closedCaptionFormatDescription: CMClosedCaptionFormatDescription, flavor: CMClosedCaptionDescriptionFlavor?, blockBufferOut: UnsafeMutablePointer&lt;CMBlockBuffer?>) -> OSStatus

Copies the contents of a closed caption format description to a buffer in big-endian byte order.

func CMClosedCaptionFormatDescriptionCreateFromBigEndianClosedCaptionDescriptionBlockBuffer(allocator: CFAllocator?, bigEndianClosedCaptionDescriptionBlockBuffer: CMBlockBuffer, flavor: CMClosedCaptionDescriptionFlavor?, formatDescriptionOut: UnsafeMutablePointer&lt;CMClosedCaptionFormatDescription?>) -> OSStatus

Creates a closed caption format description from a big-endian closed caption description structure in a buffer.

func CMClosedCaptionFormatDescriptionCreateFromBigEndianClosedCaptionDescriptionData(allocator: CFAllocator?, bigEndianClosedCaptionDescriptionData: UnsafePointer&lt;UInt8>, size: Int, flavor: CMClosedCaptionDescriptionFlavor?, formatDescriptionOut: UnsafeMutablePointer&lt;CMClosedCaptionFormatDescription?>) -> OSStatus

Creates a closed caption format description from a big-endian closed caption description structure.

func CMSwapBigEndianClosedCaptionDescriptionToHost(UnsafeMutablePointer&lt;UInt8>, Int) -> OSStatus

Converts a closed caption description structure from big-endian to host-endian, in place.

