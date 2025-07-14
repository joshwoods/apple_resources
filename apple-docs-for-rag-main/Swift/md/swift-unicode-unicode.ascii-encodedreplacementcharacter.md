

- Swift
- Unicode
- Unicode.ASCII
-  encodedReplacementCharacter 

Type Property

# encodedReplacementCharacter

A unicode scalar value to be used when repairing encoding/decoding errors, as represented in this encoding.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var encodedReplacementCharacter: Unicode.ASCII.EncodedScalar { get }
```

## Discussion

If the Unicode replacement character U+FFFD is representable in this encoding, `encodedReplacementCharacter` encodes that scalar value.

