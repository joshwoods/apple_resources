

- Core Media
-  CMTextFormatDescriptionCreateFromBigEndianTextDescriptionData(allocator:bigEndianTextDescriptionData:size:flavor:mediaType:formatDescriptionOut:) 

Function

# CMTextFormatDescriptionCreateFromBigEndianTextDescriptionData(allocator:bigEndianTextDescriptionData:size:flavor:mediaType:formatDescriptionOut:)

Creates a text format description from a big-endian text description structure.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMTextFormatDescriptionCreateFromBigEndianTextDescriptionData(
    allocator: CFAllocator?,
    bigEndianTextDescriptionData textDescriptionData: UnsafePointer,
    size: Int,
    flavor: CMTextDescriptionFlavor?,
    mediaType: CMMediaType,
    formatDescriptionOut: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`allocator`  

Allocator to use for allocating the CMTextFormatDescription object. May be NULL.

`textDescriptionData`  

TextDescription data structure in big-endian byte ordering.

`size`  

Size of TextDescription data structure.

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

func CMTextFormatDescriptionCreateFromBigEndianTextDescriptionBlockBuffer(allocator: CFAllocator?, bigEndianTextDescriptionBlockBuffer: CMBlockBuffer, flavor: CMTextDescriptionFlavor?, mediaType: CMMediaType, formatDescriptionOut: UnsafeMutablePointer&lt;CMTextFormatDescription?>) -> OSStatus

Creates a text format description from a big-endian text description structure inside a buffer.

func CMSwapBigEndianTextDescriptionToHost(UnsafeMutablePointer&lt;UInt8>, Int) -> OSStatus

Converts a text description structure from big-endian to host-endian, in place.

func CMSwapHostEndianTextDescriptionToBig(UnsafeMutablePointer&lt;UInt8>, Int) -> OSStatus

Converts a text description structure from host-endian to big-endian, in place.

