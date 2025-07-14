

- Security
-  kSecEncodeLineLengthAttribute Deprecated

Global Variable

# kSecEncodeLineLengthAttribute

The length of encoded Base32 or Base64 lines.

macOS 10.7–13.0Deprecated

``` source
let kSecEncodeLineLengthAttribute: CFString
```

Deprecated

SecTransform is no longer supported

## Discussion

Some systems can’t handle excessively long lines, or may be defined to limit lines to specific lengths (for example RFC1421 - 64, and RFC2045 - 76).

The corresponding value may be set to any positive value using a CFNumber to limit to a specific length (values smaller then X for Base32 or Y for Base64 are assume to be X or Y), or to zero for no specific limit. Either of the string constants kSecLineLength64 (RFC1421), or kSecLineLength76 (RFC2045) may be used to set line lengths of 64 or 76 bytes.

