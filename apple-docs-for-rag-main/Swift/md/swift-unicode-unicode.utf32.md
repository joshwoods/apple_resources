

- Swift
- Unicode
-  Unicode.UTF32 

Enumeration

# Unicode.UTF32

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
enum UTF32
```

## Topics

### Structures

struct Parser

### Operators

static func == (Unicode.UTF32, Unicode.UTF32) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

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

static var encodedReplacementCharacter: Unicode.UTF32.EncodedScalar

A unicode scalar value to be used when repairing encoding/decoding errors, as represented in this encoding.

### Type Methods

static func decode(Unicode.UTF32.EncodedScalar) -> Unicode.Scalar

Converts from encoded to encoding-independent representation

static func encode(Unicode.Scalar) -> Unicode.UTF32.EncodedScalar?

Converts from encoding-independent to encoded representation, returning `nil` if the scalar can’t be represented in this encoding.

static func isASCII(Unicode.UTF32.CodeUnit) -> Bool

Returns whether the given code unit represents an ASCII scalar

### Default Implementations

Equatable Implementations

UnicodeCodec Implementations

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- Equatable
- Hashable
- Sendable
- UnicodeCodec

## See Also

### Unicode Codecs

protocol UnicodeCodec

A Unicode encoding form that translates between Unicode scalar values and form-specific code units.

enum ASCII

enum UTF8

enum UTF16

enum UnicodeDecodingResult

The result of one Unicode decoding step.

enum ParseResult

The result of attempting to parse a `T` from some input.

