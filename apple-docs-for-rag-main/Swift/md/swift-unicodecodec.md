

- Swift
-  UnicodeCodec 

Protocol

# UnicodeCodec

A Unicode encoding form that translates between Unicode scalar values and form-specific code units.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol UnicodeCodec : _UnicodeEncoding
```

## Overview

The `UnicodeCodec` protocol declares methods that decode code unit sequences into Unicode scalar values and encode Unicode scalar values into code unit sequences. The standard library implements codecs for the UTF-8, UTF-16, and UTF-32 encoding schemes as the `UTF8`, `UTF16`, and `UTF32` types, respectively. Use the `Unicode.Scalar` type to work with decoded Unicode scalar values.

## Topics

### Initializers

init()

Creates an instance of the codec.

**Required**

### Instance Methods

func decode&lt;I>(inout I) -> UnicodeDecodingResult

Starts or continues decoding a code unit sequence into Unicode scalar values.

**Required**

### Type Methods

static func encode(Unicode.Scalar, into: (Self.CodeUnit) -> Void)

Encodes a Unicode scalar as a series of code units by calling the given closure on each code unit.

**Required**

## Relationships

### Conforming Types

- Unicode.UTF16
- Unicode.UTF32
- Unicode.UTF8

## See Also

### Unicode Codecs

enum ASCII

enum UTF8

enum UTF16

enum UTF32

enum UnicodeDecodingResult

The result of one Unicode decoding step.

enum ParseResult

The result of attempting to parse a `T` from some input.

