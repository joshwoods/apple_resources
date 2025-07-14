

- Core Media
-  CMClosedCaptionFormatDescriptionCreateFromBigEndianClosedCaptionDescriptionData(allocator:bigEndianClosedCaptionDescriptionData:size:flavor:formatDescriptionOut:) 

Function

# CMClosedCaptionFormatDescriptionCreateFromBigEndianClosedCaptionDescriptionData(allocator:bigEndianClosedCaptionDescriptionData:size:flavor:formatDescriptionOut:)

Creates a closed caption format description from a big-endian closed caption description structure.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMClosedCaptionFormatDescriptionCreateFromBigEndianClosedCaptionDescriptionData(
    allocator: CFAllocator?,
    bigEndianClosedCaptionDescriptionData closedCaptionDescriptionData: UnsafePointer,
    size: Int,
    flavor: CMClosedCaptionDescriptionFlavor?,
    formatDescriptionOut: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`allocator`  

Allocator to use for allocating the `CMClosedCaptionFormatDescription` object. May be `NULL`.

`closedCaptionDescriptionData`  

ClosedCaptionDescription data structure in big-endian byte ordering.

`size`  

Size of ClosedCaptionDescription data structure.

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

func CMClosedCaptionFormatDescriptionCreateFromBigEndianClosedCaptionDescriptionBlockBuffer(allocator: CFAllocator?, bigEndianClosedCaptionDescriptionBlockBuffer: CMBlockBuffer, flavor: CMClosedCaptionDescriptionFlavor?, formatDescriptionOut: UnsafeMutablePointer&lt;CMClosedCaptionFormatDescription?>) -> OSStatus

Creates a closed caption format description from a big-endian closed caption description structure in a buffer.

func CMSwapHostEndianClosedCaptionDescriptionToBig(UnsafeMutablePointer&lt;UInt8>, Int) -> OSStatus

Converts a closed caption description structure from host-endian to big-endian, in place.

func CMSwapBigEndianClosedCaptionDescriptionToHost(UnsafeMutablePointer&lt;UInt8>, Int) -> OSStatus

Converts a closed caption description structure from big-endian to host-endian, in place.

