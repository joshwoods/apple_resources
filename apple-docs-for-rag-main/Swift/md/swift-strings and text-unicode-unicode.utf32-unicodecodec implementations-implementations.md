

- Swift
- Swift Standard Library
- 
  - Swift Standard Library
- Strings and Text
- Unicode
- Unicode.UTF32
-  UnicodeCodec Implementations 

API Collection

# UnicodeCodec Implementations

## Topics

### Initializers

init()

Creates an instance of the UTF-32 codec.

### Instance Methods

func decode&lt;I>(inout I) -> UnicodeDecodingResult

Starts or continues decoding a UTF-32 sequence.

### Type Methods

static func encode(Unicode.Scalar, into: (Unicode.UTF32.CodeUnit) -> Void)

Encodes a Unicode scalar as a UTF-32 code unit by calling the given closure.

