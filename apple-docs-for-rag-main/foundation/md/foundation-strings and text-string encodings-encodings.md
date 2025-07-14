

- Foundation
- Strings and Text
-  String Encodings 

API Collection

# String Encodings

Constants for encoding standards used when converting raw data to and from string representations.

## Topics

### 7- and 8-bit Encodings

var NSASCIIStringEncoding: UInt

Strict 7-bit ASCII encoding within 8-bit chars; ASCII values 0…127 only.

var NSISOLatin1StringEncoding: UInt

8-bit ISO Latin 1 encoding.

var NSISOLatin2StringEncoding: UInt

8-bit ISO Latin 2 encoding.

var NSMacOSRomanStringEncoding: UInt

Classic Macintosh Roman encoding.

var NSNEXTSTEPStringEncoding: UInt

8-bit ASCII encoding with NEXTSTEP extensions.

var NSNonLossyASCIIStringEncoding: UInt

7-bit verbose ASCII to represent all Unicode characters.

var NSSymbolStringEncoding: UInt

8-bit Adobe Symbol encoding vector.

### 7- and 8-bit Japanese Encodings

var NSISO2022JPStringEncoding: UInt

ISO 2022 Japanese encoding for email.

var NSJapaneseEUCStringEncoding: UInt

8-bit EUC encoding for Japanese text.

var NSShiftJISStringEncoding: UInt

8-bit Shift-JIS encoding for Japanese text.

### Unicode Encodings

var NSUTF8StringEncoding: UInt

An 8-bit representation of Unicode characters, suitable for transmission or storage by ASCII-based systems.

var NSUTF16BigEndianStringEncoding: UInt

`NSUTF16StringEncoding` encoding with explicit endianness specified.

var NSUTF16LittleEndianStringEncoding: UInt

`NSUTF16StringEncoding` encoding with explicit endianness specified.

var NSUTF16StringEncoding: UInt

var NSUnicodeStringEncoding: UInt

The canonical Unicode encoding for string objects.

var NSUTF32BigEndianStringEncoding: UInt

`NSUTF32StringEncoding` encoding with explicit endianness specified.

var NSUTF32LittleEndianStringEncoding: UInt

`NSUTF32StringEncoding` encoding with explicit endianness specified.

var NSUTF32StringEncoding: UInt

32-bit UTF encoding.

### Windows Code Page Encodings

var NSWindowsCP1250StringEncoding: UInt

Microsoft Windows codepage 1250; equivalent to WinLatin2.

var NSWindowsCP1251StringEncoding: UInt

Microsoft Windows codepage 1251, encoding Cyrillic characters; equivalent to AdobeStandardCyrillic font encoding.

var NSWindowsCP1252StringEncoding: UInt

Microsoft Windows codepage 1252; equivalent to WinLatin1.

var NSWindowsCP1253StringEncoding: UInt

Microsoft Windows codepage 1253, encoding Greek characters.

var NSWindowsCP1254StringEncoding: UInt

Microsoft Windows codepage 1254, encoding Turkish characters.

## See Also

### Strings

@frozen struct String

A Unicode string value that is a collection of characters.

