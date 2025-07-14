

- Swift
-  Unicode 

Enumeration

# Unicode

A namespace for Unicode utilities.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
enum Unicode
```

## Topics

### Individual Unicode Scalar Values

struct Scalar

A Unicode scalar value.

### Unicode Scalar Classifications

enum GeneralCategory

The most general classification of a Unicode scalar.

struct CanonicalCombiningClass

The classification of a scalar used in the Canonical Ordering Algorithm defined by the Unicode Standard.

enum NumericType

The numeric type of a scalar.

### Unicode Codecs

protocol UnicodeCodec

A Unicode encoding form that translates between Unicode scalar values and form-specific code units.

enum ASCII

enum UTF8

enum UTF16

enum UTF32

enum UnicodeDecodingResult

The result of one Unicode decoding step.

enum ParseResult

The result of attempting to parse a `T` from some input.

### Translation Between Unicode Encodings

func transcode&lt;Input, InputEncoding, OutputEncoding>(Input, from: InputEncoding.Type, to: OutputEncoding.Type, stoppingOnError: Bool, into: (OutputEncoding.CodeUnit) -> Void) -> Bool

Translates the given input from one Unicode encoding to another by calling the given closure.

### Deprecated

typealias UnicodeScalar

typealias UTF8

typealias UTF16

typealias UTF32

### Type Aliases

typealias Encoding

typealias Parser

typealias Version

A version of the Unicode Standard represented by its major and minor components.

## Relationships

### Conforms To

- Sendable

