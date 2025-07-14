

- Swift
-  UnicodeDecodingResult 

Enumeration

# UnicodeDecodingResult

The result of one Unicode decoding step.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
enum UnicodeDecodingResult
```

## Overview

Each `UnicodeDecodingResult` instance can represent a Unicode scalar value, an indication that no more Unicode scalars are available, or an indication of a decoding error.

## Topics

### Operators

static func == (UnicodeDecodingResult, UnicodeDecodingResult) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case emptyInput

An indication that no more Unicode scalars are available in the input.

case error

An indication of a decoding error.

case scalarValue(Unicode.Scalar)

A decoded Unicode scalar value.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- Equatable
- Sendable

## See Also

### Unicode Codecs

protocol UnicodeCodec

A Unicode encoding form that translates between Unicode scalar values and form-specific code units.

enum ASCII

enum UTF8

enum UTF16

enum UTF32

enum ParseResult

The result of attempting to parse a `T` from some input.

