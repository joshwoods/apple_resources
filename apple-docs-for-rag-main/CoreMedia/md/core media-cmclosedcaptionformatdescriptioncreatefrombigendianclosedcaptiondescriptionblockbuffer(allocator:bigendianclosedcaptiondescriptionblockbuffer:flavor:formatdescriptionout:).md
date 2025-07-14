

- Core Media
-  CMClosedCaptionFormatDescriptionCreateFromBigEndianClosedCaptionDescriptionBlockBuffer(allocator:bigEndianClosedCaptionDescriptionBlockBuffer:flavor:formatDescriptionOut:) 

Function

# CMClosedCaptionFormatDescriptionCreateFromBigEndianClosedCaptionDescriptionBlockBuffer(allocator:bigEndianClosedCaptionDescriptionBlockBuffer:flavor:formatDescriptionOut:)

Creates a closed caption format description from a big-endian closed caption description structure in a buffer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMClosedCaptionFormatDescriptionCreateFromBigEndianClosedCaptionDescriptionBlockBuffer(
    allocator: CFAllocator?,
    bigEndianClosedCaptionDescriptionBlockBuffer closedCaptionDescriptionBlockBuffer: CMBlockBuffer,
    flavor: CMClosedCaptionDescriptionFlavor?,
    formatDescriptionOut: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`allocator`  

Allocator to use for allocating the `CMClosedCaptionFormatDescription` object. May be `NULL`.

`closedCaptionDescriptionBlockBuffer`  

`CMBlockBuffer` containing ClosedCaptionDescription data structure in big-endian byte ordering.

`flavor`  

Reserved for future use. Pass `NULL` for QuickTime Movie or ISO flavor.

`formatDescriptionOut`  

Receives new `CMClosedCaptionFormatDescription`.

## See Also

### Working with Closed Captioning Descriptions

struct CMClosedCaptionDescriptionFlavor

Types that represent closed caption format descriptions.

func CMClosedCaptionFormatDescriptionCopyAsBigEndianClosedCaptionDescriptionBlockBuffer(allocator: CFAllocator?, closedCaptionFormatDescription: CMClosedCaptionFormatDescription, flavor: CMClosedCaptionDescriptionFlavor?, blockBufferOut: UnsafeMutablePointer&lt;CMBlockBuffer?>) -> OSStatus

Copies the contents of a closed caption format description to a buffer in big-endian byte order.

func CMClosedCaptionFormatDescriptionCreateFromBigEndianClosedCaptionDescriptionData(allocator: CFAllocator?, bigEndianClosedCaptionDescriptionData: UnsafePointer&lt;UInt8>, size: Int, flavor: CMClosedCaptionDescriptionFlavor?, formatDescriptionOut: UnsafeMutablePointer&lt;CMClosedCaptionFormatDescription?>) -> OSStatus

Creates a closed caption format description from a big-endian closed caption description structure.

func CMSwapHostEndianClosedCaptionDescriptionToBig(UnsafeMutablePointer&lt;UInt8>, Int) -> OSStatus

Converts a closed caption description structure from host-endian to big-endian, in place.

func CMSwapBigEndianClosedCaptionDescriptionToHost(UnsafeMutablePointer&lt;UInt8>, Int) -> OSStatus

Converts a closed caption description structure from big-endian to host-endian, in place.

