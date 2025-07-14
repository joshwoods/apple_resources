

- Swift
- Unicode
-  Unicode.UTF8 

Enumeration

# Unicode.UTF8

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
enum UTF8
```

## Topics

### Structures

struct ForwardParser

A type that can be used to parse `CodeUnits` into `EncodedScalar`s.

struct ReverseParser

A type that can be used to parse a reversed sequence of `CodeUnits` into `EncodedScalar`s.

### Type Aliases

typealias CodeUnit

The basic unit of encoding

typealias EncodedScalar

A valid scalar value as represented in this encoding

### Type Properties

static var encodedReplacementCharacter: Unicode.UTF8.EncodedScalar

A unicode scalar value to be used when repairing encoding/decoding errors, as represented in this encoding.

### Type Methods

static func decode(Unicode.UTF8.EncodedScalar) -> Unicode.Scalar

Converts from encoded to encoding-independent representation

static func encode(Unicode.Scalar) -> Unicode.UTF8.EncodedScalar?

Converts from encoding-independent to encoded representation, returning `nil` if the scalar can’t be represented in this encoding.

static func isASCII(Unicode.UTF8.CodeUnit) -> Bool

Returns whether the given code unit represents an ASCII scalar

static func isContinuation(Unicode.UTF8.CodeUnit) -> Bool

Returns a Boolean value indicating whether the specified code unit is a UTF-8 continuation byte.

static func transcode&lt;FromEncoding>(FromEncoding.EncodedScalar, from: FromEncoding.Type) -> Unicode.UTF8.EncodedScalar?

Converts a scalar from another encoding’s representation, returning `nil` if the scalar can’t be represented in this encoding.

static func width(Unicode.Scalar) -> Int

Returns the number of code units required to encode the given Unicode scalar.

### Default Implementations

UnicodeCodec Implementations

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- Sendable
- UnicodeCodec

## See Also

### Unicode Codecs

protocol UnicodeCodec

A Unicode encoding form that translates between Unicode scalar values and form-specific code units.

enum ASCII

enum UTF16

enum UTF32

enum UnicodeDecodingResult

The result of one Unicode decoding step.

enum ParseResult

The result of attempting to parse a `T` from some input.

