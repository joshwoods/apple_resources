

- Core Media
-  CMSwapHostEndianTimeCodeDescriptionToBig(\_:\_:) 

Function

# CMSwapHostEndianTimeCodeDescriptionToBig(\_:\_:)

Converts a time code description data structure from host-endian to big-endian, in place.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMSwapHostEndianTimeCodeDescriptionToBig(
    _ timeCodeDescriptionData: UnsafeMutablePointer,
    _ timeCodeDescriptionSize: Int
) -> OSStatus
```

## Parameters 

`timeCodeDescriptionData`  

TimeCodeDescription data structure in host-endian byte ordering to be converted to big-endian byte ordering.

`timeCodeDescriptionSize`  

Size of TimeCodeDescription data structure.

## See Also

### Working with Time Code Descriptions

struct CMTimeCodeDescriptionFlavor

Types that represent time code format descriptions.

func CMTimeCodeFormatDescriptionCreate(allocator: CFAllocator?, timeCodeFormatType: CMTimeCodeFormatType, frameDuration: CMTime, frameQuanta: UInt32, flags: UInt32, extensions: CFDictionary?, formatDescriptionOut: UnsafeMutablePointer&lt;CMTimeCodeFormatDescription?>) -> OSStatus

Creates a format description for time code media.

func CMTimeCodeFormatDescriptionGetFrameDuration(CMTimeCodeFormatDescription) -> CMTime

Returns the duration of each frame.

func CMTimeCodeFormatDescriptionGetFrameQuanta(CMTimeCodeFormatDescription) -> UInt32

Returns the frames per second for a time code, or frames per tick in counter mode.

func CMTimeCodeFormatDescriptionGetTimeCodeFlags(CMTimeCodeFormatDescription) -> UInt32

Returns time code flags.

func CMTimeCodeFormatDescriptionCopyAsBigEndianTimeCodeDescriptionBlockBuffer(allocator: CFAllocator?, timeCodeFormatDescription: CMTimeCodeFormatDescription, flavor: CMTimeCodeDescriptionFlavor?, blockBufferOut: UnsafeMutablePointer&lt;CMBlockBuffer?>) -> OSStatus

Copies the contents of a time code format description to a buffer in big-endian byte order.

func CMTimeCodeFormatDescriptionCreateFromBigEndianTimeCodeDescriptionBlockBuffer(allocator: CFAllocator?, bigEndianTimeCodeDescriptionBlockBuffer: CMBlockBuffer, flavor: CMTimeCodeDescriptionFlavor?, formatDescriptionOut: UnsafeMutablePointer&lt;CMTimeCodeFormatDescription?>) -> OSStatus

Creates a time code format description from a big-endian time code description data structure in a buffer.

func CMTimeCodeFormatDescriptionCreateFromBigEndianTimeCodeDescriptionData(allocator: CFAllocator?, bigEndianTimeCodeDescriptionData: UnsafePointer&lt;UInt8>, size: Int, flavor: CMTimeCodeDescriptionFlavor?, formatDescriptionOut: UnsafeMutablePointer&lt;CMTimeCodeFormatDescription?>) -> OSStatus

Creates a time code format description from a big-endian time code description structure.

func CMSwapBigEndianTimeCodeDescriptionToHost(UnsafeMutablePointer&lt;UInt8>, Int) -> OSStatus

Converts a time code description data structure from big-endian to host-endian, in place.

