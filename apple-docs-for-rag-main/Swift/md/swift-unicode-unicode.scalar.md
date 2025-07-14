

- Swift
- Unicode
-  Unicode.Scalar 

Structure

# Unicode.Scalar

A Unicode scalar value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct Scalar
```

## Overview

The `Unicode.Scalar` type, representing a single Unicode scalar value, is the element type of a string’s `unicodeScalars` collection.

You can create a `Unicode.Scalar` instance by using a string literal that contains a single character representing exactly one Unicode scalar value.

```
let letterK: Unicode.Scalar = "K"
let kim: Unicode.Scalar = "김"
print(letterK, kim)
// Prints "K 김"
```

You can also create Unicode scalar values directly from their numeric representation.

```
let airplane = Unicode.Scalar(9992)!
print(airplane)
// Prints "✈︎"
```

## Topics

### Creating a Scalar

init(UInt8)

Creates a Unicode scalar with the specified numeric value.

init(Unicode.Scalar)

Creates a duplicate of the given Unicode scalar.

init?(UInt32)

Creates a Unicode scalar with the specified numeric value.

init?(UInt16)

Creates a Unicode scalar with the specified numeric value.

init?(Int)

Creates a Unicode scalar with the specified numeric value.

init(unicodeScalarLiteral: Unicode.Scalar)

Creates a Unicode scalar with the specified value.

init?(String)

Instantiates an instance of the conforming type from a string representation.

### Inspecting a Scalar

var value: UInt32

A numeric representation of the Unicode scalar.

var properties: Unicode.Scalar.Properties

Properties of this scalar defined by the Unicode standard.

struct Properties

A value that provides access to properties of a Unicode scalar that are defined by the Unicode standard.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

var isASCII: Bool

A Boolean value indicating whether the Unicode scalar is an ASCII character.

### Printing and Displaying a Scalar

var description: String

A textual representation of the Unicode scalar.

func write&lt;Target>(to: inout Target)

Writes the textual representation of the Unicode scalar into the given output stream.

func escaped(asASCII: Bool) -> String

Returns a string representation of the Unicode scalar.

var utf16: Unicode.Scalar.UTF16View

struct UTF16View

var debugDescription: String

An escaped textual representation of the Unicode scalar, suitable for debugging.

var customMirror: Mirror

A mirror that reflects the `Unicode.Scalar` instance.

var customPlaygroundQuickLook: _PlaygroundQuickLook

A custom playground Quick Look for the `Unicode.Scalar` instance.

Deprecated

### Comparing Scalars

static func == (Unicode.Scalar, Unicode.Scalar) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

static func &lt; (Unicode.Scalar, Unicode.Scalar) -> Bool

Returns a Boolean value indicating whether the value of the first argument is less than that of the second argument.

static func &lt;= (Self, Self) -> Bool

Returns a Boolean value indicating whether the value of the first argument is less than or equal to that of the second argument.

static func > (Self, Self) -> Bool

Returns a Boolean value indicating whether the value of the first argument is greater than that of the second argument.

static func >= (Self, Self) -> Bool

Returns a Boolean value indicating whether the value of the first argument is greater than or equal to that of the second argument.

### Creating Ranges of Scalars

static func ... (Self) -> PartialRangeFrom&lt;Self>

Returns a partial range extending upward from a lower bound.

static func ... (Self) -> PartialRangeThrough&lt;Self>

Returns a partial range up to, and including, its upper bound.

static func ... (Self, Self) -> ClosedRange&lt;Self>

Returns a closed range that contains both of its bounds.

static func ..&lt; (Self) -> PartialRangeUpTo&lt;Self>

Returns a partial range up to, but not including, its upper bound.

static func ..&lt; (Self, Self) -> Range&lt;Self>

Returns a half-open range that contains its lower bound but not its upper bound.

### Structures

struct UTF8View

### Instance Properties

var utf8: Unicode.Scalar.UTF8View

### Type Aliases

typealias Output

### Default Implementations

Comparable Implementations

CustomDebugStringConvertible Implementations

CustomReflectable Implementations

CustomStringConvertible Implementations

Equatable Implementations

ExpressibleByUnicodeScalarLiteral Implementations

Hashable Implementations

LosslessStringConvertible Implementations

RegexComponent Implementations

TextOutputStreamable Implementations

## Relationships

### Conforms To

- BitwiseCopyable
- Comparable
- Copyable
- CustomDebugStringConvertible
- CustomReflectable
- CustomStringConvertible
- Equatable
- ExpressibleByUnicodeScalarLiteral
- Hashable
- LosslessStringConvertible
- RegexComponent
- Sendable
- TextOutputStreamable

