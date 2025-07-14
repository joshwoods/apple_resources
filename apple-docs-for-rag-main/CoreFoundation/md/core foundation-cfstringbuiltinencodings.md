

- Core Foundation
-  CFStringBuiltInEncodings 

Enumeration

# CFStringBuiltInEncodings

Encodings that are built-in on all platforms on which macOS runs.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum CFStringBuiltInEncodings
```

## Topics

### Constants

case macRoman

An encoding constant that identifies the Mac Roman encoding.

case windowsLatin1

An encoding constant that identifies the Windows Latin 1 encoding (ANSI codepage 1252).

case isoLatin1

An encoding constant that identifies the ISO Latin 1 encoding (ISO 8859-1)

case nextStepLatin

An encoding constant that identifies the NextStep/OpenStep encoding.

case ASCII

An encoding constant that identifies the ASCII encoding (decimal values 0 through 127).

case unicode

An encoding constant that identifies the Unicode encoding.

case UTF8

An encoding constant that identifies the UTF 8 encoding.

case nonLossyASCII

An encoding constant that identifies non-lossy ASCII encoding.

static var UTF16: CFStringBuiltInEncodings

An encoding constant that identifies kTextEncodingUnicodeDefault + kUnicodeUTF16Format encoding (alias of kCFStringEncodingUnicode).

case UTF16BE

An encoding constant that identifies kTextEncodingUnicodeDefault + kUnicodeUTF16BEFormat encoding. This constant specifies big-endian byte order.

case UTF16LE

An encoding constant that identifies kTextEncodingUnicodeDefault + kUnicodeUTF16LEFormat encoding. This constant specifies little-endian byte order.

case UTF32

An encoding constant that identifies kTextEncodingUnicodeDefault + kUnicodeUTF32Format encoding.

case UTF32BE

An encoding constant that identifies kTextEncodingUnicodeDefault + kUnicodeUTF32BEFormat encoding. This constant specifies big-endian byte order.

case UTF32LE

An encoding constant that identifies kTextEncodingUnicodeDefault + kUnicodeUTF32LEFormat encoding. This constant specifies little-endian byte order.

### Initializers

init?(rawValue: CFStringEncoding)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

String Comparison Flags

Flags that specify how string comparisons are performed.

Invalid String Encoding Flag

Special value returned from functions to indicate a string encoding that is not supported or recognized by CFString.

External String Encodings

`CFStringEncoding` constants for encodings that may be supported by CFString.

