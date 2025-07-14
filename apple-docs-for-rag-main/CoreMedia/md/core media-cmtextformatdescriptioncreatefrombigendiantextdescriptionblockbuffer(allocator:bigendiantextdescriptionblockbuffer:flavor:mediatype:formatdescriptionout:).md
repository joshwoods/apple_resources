

- Core Media
-  CMTextFormatDescriptionCreateFromBigEndianTextDescriptionBlockBuffer(allocator:bigEndianTextDescriptionBlockBuffer:flavor:mediaType:formatDescriptionOut:) 

Function

# CMTextFormatDescriptionCreateFromBigEndianTextDescriptionBlockBuffer(allocator:bigEndianTextDescriptionBlockBuffer:flavor:mediaType:formatDescriptionOut:)

Creates a text format description from a big-endian text description structure inside a buffer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMTextFormatDescriptionCreateFromBigEndianTextDescriptionBlockBuffer(
    allocator: CFAllocator?,
    bigEndianTextDescriptionBlockBuffer textDescriptionBlockBuffer: CMBlockBuffer,
    flavor: CMTextDescriptionFlavor?,
    mediaType: CMMediaType,
    formatDescriptionOut: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`allocator`  

Allocator to use for allocating the CMTextFormatDescription object. May be NULL.

`textDescriptionBlockBuffer`  

CMBlockBuffer containing TextDescription data structure in big-endian byte ordering.

`flavor`  

Reserved for future use. Pass NULL for QuickTime Movie or ISO flavor.

`mediaType`  

Pass kCMMediaType_Text or kCMMediaType_Subtitle.

`formatDescriptionOut`  

Receives new CMTextFormatDescription.

## See Also

### Working with Text Descriptions

struct CMTextDescriptionFlavor

Types that represent text format descriptions.

func CMTextFormatDescriptionGetDefaultStyle(CMFormatDescription, localFontIDOut: UnsafeMutablePointer&lt;UInt16>?, boldOut: UnsafeMutablePointer&lt;DarwinBoolean>?, italicOut: UnsafeMutablePointer&lt;DarwinBoolean>?, underlineOut: UnsafeMutablePointer&lt;DarwinBoolean>?, fontSizeOut: UnsafeMutablePointer&lt;CGFloat>?, colorComponentsOut: UnsafeMutablePointer&lt;CGFloat>?) -> OSStatus

Returns the default text style.

func CMTextFormatDescriptionGetDefaultTextBox(CMFormatDescription, originIsAtTopLeft: Bool, heightOfTextTrack: CGFloat, defaultTextBoxOut: UnsafeMutablePointer&lt;CGRect>) -> OSStatus

Returns the default text box.

func CMTextFormatDescriptionGetDisplayFlags(CMFormatDescription, displayFlagsOut: UnsafeMutablePointer&lt;CMTextDisplayFlags>) -> OSStatus

Returns the display flags.

func CMTextFormatDescriptionGetFontName(CMFormatDescription, localFontID: UInt16, fontNameOut: AutoreleasingUnsafeMutablePointer&lt;CFString?>) -> OSStatus

Returns a font name for a local font identifier.

func CMTextFormatDescriptionGetJustification(CMFormatDescription, horizontalOut: UnsafeMutablePointer&lt;CMTextJustificationValue>?, verticalOut: UnsafeMutablePointer&lt;CMTextJustificationValue>?) -> OSStatus

Returns the horizontal and vertical justification.

func CMTextFormatDescriptionCopyAsBigEndianTextDescriptionBlockBuffer(allocator: CFAllocator?, textFormatDescription: CMTextFormatDescription, flavor: CMTextDescriptionFlavor?, blockBufferOut: UnsafeMutablePointer&lt;CMBlockBuffer?>) -> OSStatus

Copies the contents of a text format description to a buffer in big-endian byte order.

func CMTextFormatDescriptionCreateFromBigEndianTextDescriptionData(allocator: CFAllocator?, bigEndianTextDescriptionData: UnsafePointer&lt;UInt8>, size: Int, flavor: CMTextDescriptionFlavor?, mediaType: CMMediaType, formatDescriptionOut: UnsafeMutablePointer&lt;CMTextFormatDescription?>) -> OSStatus

Creates a text format description from a big-endian text description structure.

func CMSwapBigEndianTextDescriptionToHost(UnsafeMutablePointer&lt;UInt8>, Int) -> OSStatus

Converts a text description structure from big-endian to host-endian, in place.

func CMSwapHostEndianTextDescriptionToBig(UnsafeMutablePointer&lt;UInt8>, Int) -> OSStatus

Converts a text description structure from host-endian to big-endian, in place.

