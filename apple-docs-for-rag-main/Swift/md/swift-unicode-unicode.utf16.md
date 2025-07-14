

- Swift
- Unicode
-  Unicode.UTF16 

Enumeration

# Unicode.UTF16

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
enum UTF16
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

static var encodedReplacementCharacter: Unicode.UTF16.EncodedScalar

A unicode scalar value to be used when repairing encoding/decoding errors, as represented in this encoding.

### Type Methods

static func decode(Unicode.UTF16.EncodedScalar) -> Unicode.Scalar

Converts from encoded to encoding-independent representation

static func encode(Unicode.Scalar) -> Unicode.UTF16.EncodedScalar?

Converts from encoding-independent to encoded representation, returning `nil` if the scalar can’t be represented in this encoding.

static func isASCII(Unicode.UTF16.CodeUnit) -> Bool

Returns whether the given code unit represents an ASCII scalar

static func isLeadSurrogate(Unicode.UTF16.CodeUnit) -> Bool

Returns a Boolean value indicating whether the specified code unit is a high-surrogate code unit.

static func isSurrogate(Unicode.UTF16.CodeUnit) -> Bool

Returns a Boolean value indicating whether the specified code unit is a high or low surrogate code unit.

static func isTrailSurrogate(Unicode.UTF16.CodeUnit) -> Bool

Returns a Boolean value indicating whether the specified code unit is a low-surrogate code unit.

static func leadSurrogate(Unicode.Scalar) -> UTF16.CodeUnit

Returns the high-surrogate code unit of the surrogate pair representing the specified Unicode scalar.

static func trailSurrogate(Unicode.Scalar) -> UTF16.CodeUnit

Returns the low-surrogate code unit of the surrogate pair representing the specified Unicode scalar.

static func transcode&lt;FromEncoding>(FromEncoding.EncodedScalar, from: FromEncoding.Type) -> Unicode.UTF16.EncodedScalar?

Converts a scalar from another encoding’s representation, returning `nil` if the scalar can’t be represented in this encoding.

static func transcodedLength&lt;Input, Encoding>(of: Input, decodedAs: Encoding.Type, repairingIllFormedSequences: Bool) -> (count: Int, isASCII: Bool)?

Returns the number of UTF-16 code units required for the given code unit sequence when transcoded to UTF-16, and a Boolean value indicating whether the sequence was found to contain only ASCII characters.

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

enum UTF8

enum UTF32

enum UnicodeDecodingResult

The result of one Unicode decoding step.

enum ParseResult

The result of attempting to parse a `T` from some input.

