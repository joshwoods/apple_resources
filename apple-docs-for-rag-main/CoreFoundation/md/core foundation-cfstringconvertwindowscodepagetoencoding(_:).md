

- Core Foundation
-  CFStringConvertWindowsCodepageToEncoding(\_:) 

Function

# CFStringConvertWindowsCodepageToEncoding(\_:)

Returns the Core Foundation encoding constant that is the closest mapping to a given Windows codepage identifier.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFStringConvertWindowsCodepageToEncoding(_ codepage: UInt32) -> CFStringEncoding
```

## Parameters 

`codepage`  

The Windows codepage identifier to use.

## Return Value

The Core Foundation string encoding that is closest to the Windows codepage identifier `codepage`. Returns the kCFStringEncodingInvalidId constant if the mapping is not known.

## Discussion

The CFStringConvertEncodingToWindowsCodepage(_:) function is complementary to this function.

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

func CFStringGetFastestEncoding(CFString!) -> CFStringEncoding

Returns for a CFString object the character encoding that requires the least conversion time.

func CFStringGetListOfAvailableEncodings() -> UnsafePointer&lt;CFStringEncoding>!

Returns a pointer to a list of string encodings supported by the current system.

func CFStringGetMaximumSizeForEncoding(CFIndex, CFStringEncoding) -> CFIndex

Returns the maximum number of bytes a string of a specified length (in Unicode characters) will take up if encoded in a specified encoding.

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

