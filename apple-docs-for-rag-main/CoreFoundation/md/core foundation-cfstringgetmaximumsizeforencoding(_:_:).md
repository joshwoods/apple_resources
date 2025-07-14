

- Core Foundation
-  CFStringGetMaximumSizeForEncoding(\_:\_:) 

Function

# CFStringGetMaximumSizeForEncoding(\_:\_:)

Returns the maximum number of bytes a string of a specified length (in Unicode characters) will take up if encoded in a specified encoding.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFStringGetMaximumSizeForEncoding(
    _ length: CFIndex,
    _ encoding: CFStringEncoding
) -> CFIndex
```

## Parameters 

`length`  

The number of Unicode characters to evaluate.

`encoding`  

The string encoding for the number of characters specified by `length`.

## Return Value

The maximum number of bytes that could be needed to represent `length` number of Unicode characters with the string encoding `encoding`, or kCFNotFound if the number exceeds `LONG_MAX`.

## Discussion

The number of bytes that the encoding actually ends up requiring when converting any particular string could be less than the returned value, but never more.

## See Also

### Working With Encodings

func CFStringConvertEncodingToIANACharSetName(CFStringEncoding) -> CFString!

Returns the name of the IANA registry “charset” that is the closest mapping to a specified string encoding.

func CFStringConvertEncodingToNSStringEncoding(CFStringEncoding) -> UInt

Returns the Cocoa encoding constant that maps most closely to a given Core Foundation encoding constant.

func CFStringConvertEncodingToWindowsCodepage(CFStringEncoding) -> UInt32

Returns the Windows codepage identifier that maps most closely to a given Core Foundation encoding constant.

func CFStringConvertIANACharSetNameToEncoding(CFString!) -> CFStringEncoding

Returns the Core Foundation encoding constant that is the closest mapping to a given IANA registry “charset” name.

func CFStringConvertNSStringEncodingToEncoding(UInt) -> CFStringEncoding

Returns the Core Foundation encoding constant that is the closest mapping to a given Cocoa encoding.

func CFStringConvertWindowsCodepageToEncoding(UInt32) -> CFStringEncoding

Returns the Core Foundation encoding constant that is the closest mapping to a given Windows codepage identifier.

func CFStringGetFastestEncoding(CFString!) -> CFStringEncoding

Returns for a CFString object the character encoding that requires the least conversion time.

func CFStringGetListOfAvailableEncodings() -> UnsafePointer&lt;CFStringEncoding>!

Returns a pointer to a list of string encodings supported by the current system.

func CFStringGetMostCompatibleMacStringEncoding(CFStringEncoding) -> CFStringEncoding

Returns the most compatible Mac OS script value for the given input encoding.

func CFStringGetNameOfEncoding(CFStringEncoding) -> CFString!

Returns the canonical name of a specified string encoding.

func CFStringGetSmallestEncoding(CFString!) -> CFStringEncoding

Returns the smallest encoding on the current system for the character contents of a string.

func CFStringGetSystemEncoding() -> CFStringEncoding

Returns the default encoding used by the operating system when it creates strings.

func CFStringIsEncodingAvailable(CFStringEncoding) -> Bool

Determines whether a given Core Foundation string encoding is available on the current system.

