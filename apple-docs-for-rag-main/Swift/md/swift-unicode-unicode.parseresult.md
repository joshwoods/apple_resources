

- Swift
- Unicode
-  Unicode.ParseResult 

Enumeration

# Unicode.ParseResult

The result of attempting to parse a `T` from some input.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
enum ParseResult
```

## Topics

### Enumeration Cases

case emptyInput

The input was entirely consumed.

case error(length: Int)

An encoding error was detected.

case valid(T)

A `T` was parsed successfully

## Relationships

### Conforms To

- Sendable

  Conforms when `T` conforms to `Copyable`, `Escapable`, and `Sendable`.

## See Also

### Unicode Codecs

protocol UnicodeCodec

A Unicode encoding form that translates between Unicode scalar values and form-specific code units.

enum ASCII

enum UTF8

enum UTF16

enum UTF32

enum UnicodeDecodingResult

The result of one Unicode decoding step.

