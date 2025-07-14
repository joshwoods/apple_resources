

- Core Media
-  CMTextFormatDescriptionGetFontName(\_:localFontID:fontNameOut:) 

Function

# CMTextFormatDescriptionGetFontName(\_:localFontID:fontNameOut:)

Returns a font name for a local font identifier.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMTextFormatDescriptionGetFontName(
    _ desc: CMFormatDescription,
    localFontID: UInt16,
    fontNameOut: AutoreleasingUnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`desc`  

`CMFormatDescription` being interrogated.

`localFontID`  

Font number, local to the FormatDescription.

`fontNameOut`  

On output, returns name of the font. The returned font is not retained by this call, so clients are required to retain it if they need to keep it longer.

## Return Value

A result code. Returns `noErr` if successful.

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

func CMTextFormatDescriptionGetJustification(CMFormatDescription, horizontalOut: UnsafeMutablePointer&lt;CMTextJustificationValue>?, verticalOut: UnsafeMutablePointer&lt;CMTextJustificationValue>?) -> OSStatus

Returns the horizontal and vertical justification.

func CMTextFormatDescriptionCopyAsBigEndianTextDescriptionBlockBuffer(allocator: CFAllocator?, textFormatDescription: CMTextFormatDescription, flavor: CMTextDescriptionFlavor?, blockBufferOut: UnsafeMutablePointer&lt;CMBlockBuffer?>) -> OSStatus

Copies the contents of a text format description to a buffer in big-endian byte order.

func CMTextFormatDescriptionCreateFromBigEndianTextDescriptionBlockBuffer(allocator: CFAllocator?, bigEndianTextDescriptionBlockBuffer: CMBlockBuffer, flavor: CMTextDescriptionFlavor?, mediaType: CMMediaType, formatDescriptionOut: UnsafeMutablePointer&lt;CMTextFormatDescription?>) -> OSStatus

Creates a text format description from a big-endian text description structure inside a buffer.

func CMTextFormatDescriptionCreateFromBigEndianTextDescriptionData(allocator: CFAllocator?, bigEndianTextDescriptionData: UnsafePointer&lt;UInt8>, size: Int, flavor: CMTextDescriptionFlavor?, mediaType: CMMediaType, formatDescriptionOut: UnsafeMutablePointer&lt;CMTextFormatDescription?>) -> OSStatus

Creates a text format description from a big-endian text description structure.

func CMSwapBigEndianTextDescriptionToHost(UnsafeMutablePointer&lt;UInt8>, Int) -> OSStatus

Converts a text description structure from big-endian to host-endian, in place.

func CMSwapHostEndianTextDescriptionToBig(UnsafeMutablePointer&lt;UInt8>, Int) -> OSStatus

Converts a text description structure from host-endian to big-endian, in place.

