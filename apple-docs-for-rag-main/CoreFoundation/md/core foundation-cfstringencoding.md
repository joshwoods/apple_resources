

- Core Foundation
-  CFStringEncoding 

Type Alias

# CFStringEncoding

An integer type for constants used to specify supported string encodings in various CFString functions.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias CFStringEncoding = UInt32
```

## Discussion

This type is used to define the constants for the built-in encodings (see CFStringBuiltInEncodings for a list) and for platform-dependent encodings (see External String Encodings). If CFString does not recognize or support the string encoding of a particular string, CFString functions will identify the string’s encoding as kCFStringEncodingInvalidId.

## See Also

### Data Types

enum CFStringEncodings

Index type for constants used to specify external string encodings.

struct CFStringCompareFlags

A CFOptionFlags type for specifying options for string comparison .

struct CFStringInlineBuffer

Defines the buffer and related fields used for in-line buffer access of characters in CFString objects.

