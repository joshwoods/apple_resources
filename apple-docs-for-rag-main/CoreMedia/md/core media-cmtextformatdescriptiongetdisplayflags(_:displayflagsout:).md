

- Core Media
-  CMTextFormatDescriptionGetDisplayFlags(\_:displayFlagsOut:) 

Function

# CMTextFormatDescriptionGetDisplayFlags(\_:displayFlagsOut:)

Returns the display flags.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMTextFormatDescriptionGetDisplayFlags(
    _ desc: CMFormatDescription,
    displayFlagsOut: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`desc`  

`CMFormatDescription` being interrogated.

`displayFlagsOut`  

On output, receives the display flags.

## Return Value

A result code. Returns `noErr` if successful.

## Discussion

These are the flags that control how the text appears.

## See Also

### Working with Text Descriptions

struct CMTextDescriptionFlavor

Types that represent text format descriptions.

func CMTextFormatDescriptionGetDefaultStyle(CMFormatDescription, localFontIDOut: UnsafeMutablePointer&lt;UInt16>?, boldOut: UnsafeMutablePointer&lt;DarwinBoolean>?, italicOut: UnsafeMutablePointer&lt;DarwinBoolean>?, underlineOut: UnsafeMutablePointer&lt;DarwinBoolean>?, fontSizeOut: UnsafeMutablePointer&lt;CGFloat>?, colorComponentsOut: UnsafeMutablePointer&lt;CGFloat>?) -> OSStatus

Returns the default text style.

func CMTextFormatDescriptionGetDefaultTextBox(CMFormatDescription, originIsAtTopLeft: Bool, heightOfTextTrack: CGFloat, defaultTextBoxOut: UnsafeMutablePointer&lt;CGRect>) -> OSStatus

Returns the default text box.

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

