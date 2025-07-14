

- Core Media
-  CMMetadataFormatDescriptionCopyAsBigEndianMetadataDescriptionBlockBuffer(allocator:metadataFormatDescription:flavor:blockBufferOut:) 

Function

# CMMetadataFormatDescriptionCopyAsBigEndianMetadataDescriptionBlockBuffer(allocator:metadataFormatDescription:flavor:blockBufferOut:)

Copies the contents of a metadata format description to a buffer in big-endian byte order.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMMetadataFormatDescriptionCopyAsBigEndianMetadataDescriptionBlockBuffer(
    allocator: CFAllocator?,
    metadataFormatDescription: CMMetadataFormatDescription,
    flavor: CMMetadataDescriptionFlavor?,
    blockBufferOut: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`allocator`  

Allocator to use for allocating the CMBlockBuffer object. May be NULL.

`metadataFormatDescription`  

CMMetadataFormatDescriptionRef to be copied.

`flavor`  

Reserved for future use. Pass NULL for QuickTime Movie or ISO flavor.

`blockBufferOut`  

Receives new CMBlockBuffer containing MetadataDescription data structure in big-endian byte ordering.

## Discussion

On return, the caller owns the returned CMBlockBuffer, and must release it when done with it.

Note

The `dataRefIndex` field of the SampleDescription is intentionally filled with garbage values (`0xFFFF`). The caller must overwrite these values with a valid `dataRefIndex` if writing the SampleDescription to a QuickTime/ISO file.

## See Also

### Working with Metadata Descriptions

struct CMMetadataDescriptionFlavor

Types that represent metadata format descriptions.

func CMMetadataFormatDescriptionCreateWithKeys(allocator: CFAllocator?, metadataType: CMMetadataFormatType, keys: CFArray?, formatDescriptionOut: UnsafeMutablePointer&lt;CMMetadataFormatDescription?>) -> OSStatus

Creates a metadata format description with the metadata keys you specify.

func CMMetadataFormatDescriptionGetKeyWithLocalID(CMMetadataFormatDescription, localKeyID: OSType) -> CFDictionary?

Returns the key for the local identifier.

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

