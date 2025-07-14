

- Core Media
-  CMMetadataDescriptionFlavor 

Structure

# CMMetadataDescriptionFlavor

Types that represent metadata format descriptions.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
struct CMMetadataDescriptionFlavor
```

## Topics

### Creating Metadata Description Flavors

init(CFString)

Creates a metadata description flavor.

init(rawValue: CFString)

Creates a metadata description flavor.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Working with Metadata Descriptions

func CMMetadataFormatDescriptionCreateWithKeys(allocator: CFAllocator?, metadataType: CMMetadataFormatType, keys: CFArray?, formatDescriptionOut: UnsafeMutablePointer&lt;CMMetadataFormatDescription?>) -> OSStatus

Creates a metadata format description with the metadata keys you specify.

func CMMetadataFormatDescriptionGetKeyWithLocalID(CMMetadataFormatDescription, localKeyID: OSType) -> CFDictionary?

Returns the key for the local identifier.

func CMMetadataFormatDescriptionCopyAsBigEndianMetadataDescriptionBlockBuffer(allocator: CFAllocator?, metadataFormatDescription: CMMetadataFormatDescription, flavor: CMMetadataDescriptionFlavor?, blockBufferOut: UnsafeMutablePointer&lt;CMBlockBuffer?>) -> OSStatus

Copies the contents of a metadata format description to a buffer in big-endian byte order.

func CMMetadataFormatDescriptionCreateByMergingMetadataFormatDescriptions(allocator: CFAllocator?, sourceDescription: CMMetadataFormatDescription, otherSourceDescription: CMMetadataFormatDescription, formatDescriptionOut: UnsafeMutablePointer&lt;CMMetadataFormatDescription?>) -> OSStatus

Creates a metadata format description object by merging with another description.

func CMMetadataFormatDescriptionCreateFromBigEndianMetadataDescriptionBlockBuffer(allocator: CFAllocator?, bigEndianMetadataDescriptionBlockBuffer: CMBlockBuffer, flavor: CMMetadataDescriptionFlavor?, formatDescriptionOut: UnsafeMutablePointer&lt;CMMetadataFormatDescription?>) -> OSStatus

Creates a metadata format description from a big-endian metadata description structure inside a buffer.

func CMMetadataFormatDescriptionCreateFromBigEndianMetadataDescriptionData(allocator: CFAllocator?, bigEndianMetadataDescriptionData: UnsafePointer&lt;UInt8>, size: Int, flavor: CMMetadataDescriptionFlavor?, formatDescriptionOut: UnsafeMutablePointer&lt;CMMetadataFormatDescription?>) -> OSStatus

Creates a metadata format description from a big-endian metadata description structure.

func CMMetadataFormatDescriptionCreateWithMetadataFormatDescriptionAndMetadataSpecifications(allocator: CFAllocator?, sourceDescription: CMMetadataFormatDescription, metadataSpecifications: CFArray, formatDescriptionOut: UnsafeMutablePointer&lt;CMMetadataFormatDescription?>) -> OSStatus

Creates a metadata format description by extending an existing description with the values you specify.

func CMMetadataFormatDescriptionCreateWithMetadataSpecifications(allocator: CFAllocator?, metadataType: CMMetadataFormatType, metadataSpecifications: CFArray, formatDescriptionOut: UnsafeMutablePointer&lt;CMMetadataFormatDescription?>) -> OSStatus

Creates a metadata format description with the specifications you specify.

func CMSwapBigEndianMetadataDescriptionToHost(UnsafeMutablePointer&lt;UInt8>, Int) -> OSStatus

Converts a metadata description data structure from big-endian to host-endian, in place.

func CMSwapHostEndianMetadataDescriptionToBig(UnsafeMutablePointer&lt;UInt8>, Int) -> OSStatus

Converts a metadata description data structure from host-endian to big-endian, in place.

func CMMetadataFormatDescriptionGetIdentifiers(CMMetadataFormatDescription) -> CFArray?

Returns an array of metadata identifiers from a metadata format description.

