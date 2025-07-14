

- Core Media
-  CMClosedCaptionDescriptionFlavor 

Structure

# CMClosedCaptionDescriptionFlavor

Types that represent closed caption format descriptions.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
struct CMClosedCaptionDescriptionFlavor
```

## Topics

### Initializers

init(CFString)

Creates a closed caption description flavor.

init(rawValue: CFString)

Creates a closed caption description flavor.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Working with Closed Captioning Descriptions

func CMClosedCaptionFormatDescriptionCopyAsBigEndianClosedCaptionDescriptionBlockBuffer(allocator: CFAllocator?, closedCaptionFormatDescription: CMClosedCaptionFormatDescription, flavor: CMClosedCaptionDescriptionFlavor?, blockBufferOut: UnsafeMutablePointer&lt;CMBlockBuffer?>) -> OSStatus

Copies the contents of a closed caption format description to a buffer in big-endian byte order.

func CMClosedCaptionFormatDescriptionCreateFromBigEndianClosedCaptionDescriptionBlockBuffer(allocator: CFAllocator?, bigEndianClosedCaptionDescriptionBlockBuffer: CMBlockBuffer, flavor: CMClosedCaptionDescriptionFlavor?, formatDescriptionOut: UnsafeMutablePointer&lt;CMClosedCaptionFormatDescription?>) -> OSStatus

Creates a closed caption format description from a big-endian closed caption description structure in a buffer.

func CMClosedCaptionFormatDescriptionCreateFromBigEndianClosedCaptionDescriptionData(allocator: CFAllocator?, bigEndianClosedCaptionDescriptionData: UnsafePointer&lt;UInt8>, size: Int, flavor: CMClosedCaptionDescriptionFlavor?, formatDescriptionOut: UnsafeMutablePointer&lt;CMClosedCaptionFormatDescription?>) -> OSStatus

Creates a closed caption format description from a big-endian closed caption description structure.

func CMSwapHostEndianClosedCaptionDescriptionToBig(UnsafeMutablePointer&lt;UInt8>, Int) -> OSStatus

Converts a closed caption description structure from host-endian to big-endian, in place.

func CMSwapBigEndianClosedCaptionDescriptionToHost(UnsafeMutablePointer&lt;UInt8>, Int) -> OSStatus

Converts a closed caption description structure from big-endian to host-endian, in place.

