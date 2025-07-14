

- Core Media
-  CMTextFormatDescriptionGetDefaultTextBox(\_:originIsAtTopLeft:heightOfTextTrack:defaultTextBoxOut:) 

Function

# CMTextFormatDescriptionGetDefaultTextBox(\_:originIsAtTopLeft:heightOfTextTrack:defaultTextBoxOut:)

Returns the default text box.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMTextFormatDescriptionGetDefaultTextBox(
    _ desc: CMFormatDescription,
    originIsAtTopLeft: Bool,
    heightOfTextTrack: CGFloat,
    defaultTextBoxOut: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`desc`  

FormatDescription being interrogated.

`originIsAtTopLeft`  

Pass true if the `CGRect` will be used in an environment where (0,0) is at the top-left corner of an enclosing rectangle and y coordinates increase as you go down.

Pass false if the `CGRect` will be used in an environment where (0,0) is at the bottom-left corner of an enclosing rectangle and y coordinates increase as you go up.

`heightOfTextTrack`  

If `originIsAtTopLeft` is false, pass the height of the enclosing text track or destination. This value will be used to properly compute the default text box for the given origin. Ignored if `originIsAtTopLeft` is true.

`defaultTextBoxOut`  

On output, receives the default text box.

## Return Value

A result code. Returns `noErr` if successful.

## Discussion

Within a text track, text is rendered within a text box. There is a default text box set, which can be over-ridden by a sample.

## See Also

### Working with Text Descriptions

struct CMTextDescriptionFlavor

Types that represent text format descriptions.

func CMTextFormatDescriptionGetDefaultStyle(CMFormatDescription, localFontIDOut: UnsafeMutablePointer&lt;UInt16>?, boldOut: UnsafeMutablePointer&lt;DarwinBoolean>?, italicOut: UnsafeMutablePointer&lt;DarwinBoolean>?, underlineOut: UnsafeMutablePointer&lt;DarwinBoolean>?, fontSizeOut: UnsafeMutablePointer&lt;CGFloat>?, colorComponentsOut: UnsafeMutablePointer&lt;CGFloat>?) -> OSStatus

Returns the default text style.

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

