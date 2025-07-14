

- Core Media
-  CMTextFormatDescriptionGetDefaultStyle(\_:localFontIDOut:boldOut:italicOut:underlineOut:fontSizeOut:colorComponentsOut:) 

Function

# CMTextFormatDescriptionGetDefaultStyle(\_:localFontIDOut:boldOut:italicOut:underlineOut:fontSizeOut:colorComponentsOut:)

Returns the default text style.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMTextFormatDescriptionGetDefaultStyle(
    _ desc: CMFormatDescription,
    localFontIDOut: UnsafeMutablePointer?,
    boldOut: UnsafeMutablePointer?,
    italicOut: UnsafeMutablePointer?,
    underlineOut: UnsafeMutablePointer?,
    fontSizeOut: UnsafeMutablePointer?,
    colorComponentsOut: UnsafeMutablePointer?
) -> OSStatus
```

## Parameters 

`desc`  

`CMFormatDescription` being interrogated.

`localFontIDOut`  

Font number, local to the FormatDescription. May be `NULL`.

`boldOut`  

Returned true if style includes Bold. May be `NULL`.

`italicOut`  

On output, returns true if style includes Italic. May be `NULL`.

`underlineOut`  

On output, returns true if style includes Underline. May be `NULL`.

`fontSizeOut`  

FontSize in points. May be `NULL`.

`colorComponentsOut`  

Color components in order red, green, blue, and alpha. May be `NULL`.

## Return Value

A result code. Returns `noErr` if Successful.

## See Also

### Working with Text Descriptions

struct CMTextDescriptionFlavor

Types that represent text format descriptions.

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

func CMTextFormatDescriptionCreateFromBigEndianTextDescriptionData(allocator: CFAllocator?, bigEndianTextDescriptionData: UnsafePointer&lt;UInt8>, size: Int, flavor: CMTextDescriptionFlavor?, mediaType: CMMediaType, formatDescriptionOut: UnsafeMutablePointer&lt;CMTextFormatDescription?>) -> OSStatus

Creates a text format description from a big-endian text description structure.

func CMSwapBigEndianTextDescriptionToHost(UnsafeMutablePointer&lt;UInt8>, Int) -> OSStatus

Converts a text description structure from big-endian to host-endian, in place.

func CMSwapHostEndianTextDescriptionToBig(UnsafeMutablePointer&lt;UInt8>, Int) -> OSStatus

Converts a text description structure from host-endian to big-endian, in place.

