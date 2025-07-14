

- Swift
- Swift Standard Library
- 
  - Swift Standard Library
- Strings and Text
- Unicode
- Unicode.UTF8
-  UnicodeCodec Implementations 

API Collection

# UnicodeCodec Implementations

## Topics

### Initializers

init()

Creates an instance of the UTF-8 codec.

### Instance Methods

func decode&lt;I>(inout I) -> UnicodeDecodingResult

Starts or continues decoding a UTF-8 sequence.

### Type Methods

static func encode(Unicode.Scalar, into: (Unicode.UTF8.CodeUnit) -> Void)

Encodes a Unicode scalar as a series of code units by calling the given closure on each code unit.

