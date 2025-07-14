

- Swift
- Unicode
-  Unicode.ASCII 

Enumeration

# Unicode.ASCII

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
enum ASCII
```

## Topics

### Structures

struct Parser

### Type Aliases

typealias CodeUnit

The basic unit of encoding

typealias EncodedScalar

A valid scalar value as represented in this encoding

typealias ForwardParser

A type that can be used to parse `CodeUnits` into `EncodedScalar`s.

typealias ReverseParser

A type that can be used to parse a reversed sequence of `CodeUnits` into `EncodedScalar`s.

### Type Properties

static var encodedReplacementCharacter: Unicode.ASCII.EncodedScalar

A unicode scalar value to be used when repairing encoding/decoding errors, as represented in this encoding.

### Type Methods

static func decode(Unicode.ASCII.EncodedScalar) -> Unicode.Scalar

Converts from encoded to encoding-independent representation

static func encode(Unicode.Scalar) -> Unicode.ASCII.EncodedScalar?

Converts from encoding-independent to encoded representation, returning `nil` if the scalar can’t be represented in this encoding.

static func isASCII(Unicode.ASCII.CodeUnit) -> Bool

Returns whether the given code unit represents an ASCII scalar

static func transcode&lt;FromEncoding>(FromEncoding.EncodedScalar, from: FromEncoding.Type) -> Unicode.ASCII.EncodedScalar?

Converts a scalar from another encoding’s representation, returning `nil` if the scalar can’t be represented in this encoding.

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- Sendable

## See Also

### Unicode Codecs

protocol UnicodeCodec

A Unicode encoding form that translates between Unicode scalar values and form-specific code units.

enum UTF8

enum UTF16

enum UTF32

enum UnicodeDecodingResult

The result of one Unicode decoding step.

enum ParseResult

The result of attempting to parse a `T` from some input.

