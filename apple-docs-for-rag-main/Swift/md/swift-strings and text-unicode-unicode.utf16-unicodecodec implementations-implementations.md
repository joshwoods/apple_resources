

- Swift
- Swift Standard Library
- 
  - Swift Standard Library
- Strings and Text
- Unicode
- Unicode.UTF16
-  UnicodeCodec Implementations 

API Collection

# UnicodeCodec Implementations

## Topics

### Initializers

init()

Creates an instance of the UTF-16 codec.

### Instance Methods

func decode&lt;I>(inout I) -> UnicodeDecodingResult

Starts or continues decoding a UTF-16 sequence.

### Type Methods

static func encode(Unicode.Scalar, into: (Unicode.UTF16.CodeUnit) -> Void)

Encodes a Unicode scalar as a series of code units by calling the given closure on each code unit.

