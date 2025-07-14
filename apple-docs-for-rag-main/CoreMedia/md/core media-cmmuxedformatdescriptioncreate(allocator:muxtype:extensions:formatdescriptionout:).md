

- Core Media
-  CMMuxedFormatDescriptionCreate(allocator:muxType:extensions:formatDescriptionOut:) 

Function

# CMMuxedFormatDescriptionCreate(allocator:muxType:extensions:formatDescriptionOut:)

Creates a format description for a muxed media stream.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMMuxedFormatDescriptionCreate(
    allocator: CFAllocator?,
    muxType: CMMuxedStreamType,
    extensions: CFDictionary?,
    formatDescriptionOut: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`allocator`  

`CFAllocator` to be used. Pass `NULL` or `kCFAllocatorDefault` to use the default allocator.

`muxType`  

Type of the muxed stream (e.g. `kCMMuxedStreamType_MPEG2Transport` for MPEG-2 transport stream). This is the media subtype, and will be returned if you subsequently call `CMFormatDescriptionGetMediaSubType` (or `CMMuxedFormatDescriptionGetStreamType`).

`extensions`  

Dictionary of extension key/value pairs. Keys are always of type `CFString`. Values are always property list objects (i.e.. `CFData`, `CFString`, `CFArray`, `CFDictionary`, `CFDate`, `CFBoolean`, or `CFNumber`). Can be `NULL`.

`formatDescriptionOut`  

On output, returns newly created muxed `CMFormatDescription`

## Return Value

A result code. Returns `noErr` if successful.

## Discussion

A muxed format description does not know the formats of the sub-streams within the muxed stream. That information will only be discoverable by the demuxer software (or other software which understands the details of the muxed bitstream) which will need to produce separate format descriptions for each of its output streams. The caller owns the returned `CMFormatDescription`, and must release it when done with it. All input parameters are copied (the extensions are deep-copied). The caller can deallocate them or re-use them after making this call.

