

- Swift
-  Substring 

Structure

# Substring

A slice of a string.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct Substring
```

## Overview

When you create a slice of a string, a `Substring` instance is the result. Operating on substrings is fast and efficient because a substring shares its storage with the original string. The `Substring` type presents the same interface as `String`, so you can avoid or defer any copying of the string’s contents.

The following example creates a `greeting` string, and then finds the substring of the first sentence:

```
let greeting = "Hi there! It's nice to meet you! 👋"
let endOfSentence = greeting.firstIndex(of: "!")!
let firstSentence = greeting[...endOfSentence]
// firstSentence == "Hi there!"
```

You can perform many string operations on a substring. Here, we find the length of the first sentence and create an uppercase version.

```
print("'\(firstSentence)' is \(firstSentence.count) characters long.")
// Prints "'Hi there!' is 9 characters long."

let shoutingSentence = firstSentence.uppercased()
// shoutingSentence == "HI THERE!"
```

# Converting a Substring to a String

This example defines a `rawData` string with some unstructured data, and then uses the string’s `prefix(while:)` method to create a substring of the numeric prefix:

```
let rawInput = "126 a.b 22219 zzzzzz"
let numericPrefix = rawInput.prefix(while: { "0"..."9" ~= $0 })
// numericPrefix is the substring "126"
```

When you need to store a substring or pass it to a function that requires a `String` instance, you can convert it to a `String` by using the `String(_:)` initializer. Calling this initializer copies the contents of the substring to a new string.

```
func parseAndAddOne(_ s: String) -> Int {
    return Int(s, radix: 10)! + 1
}
_ = parseAndAddOne(numericPrefix)
// error: cannot convert value...
let incrementedPrefix = parseAndAddOne(String(numericPrefix))
// incrementedPrefix == 127
```

Alternatively, you can convert the function that takes a `String` to one that is generic over the `StringProtocol` protocol. The following code declares a generic version of the `parseAndAddOne(_:)` function:

```
func genericParseAndAddOne(_ s: S) -> Int {
    return Int(s, radix: 10)! + 1
}
let genericallyIncremented = genericParseAndAddOne(numericPrefix)
// genericallyIncremented == 127
```

You can call this generic function with an instance of either `String` or `Substring`.

Important

Don’t store substrings longer than you need them to perform a specific operation. A substring holds a reference to the entire storage of the string it comes from, not just to the portion it presents, even when there is no other reference to the original string. Storing substrings may, therefore, prolong the lifetime of string data that is no longer otherwise accessible, which can appear to be memory leakage.

## Topics

### Operators

static func ~= (Substring, String) -> Bool

### Initializers

init()

Creates an empty substring.

init(Substring.UTF8View)

Creates a Substring having the given content.

init(Substring.UTF16View)

Creates a Substring having the given content.

init(Substring.UnicodeScalarView)

Creates a Substring having the given content.

### Instance Properties

var base: String

Returns the underlying string from which this substring was derived.

var characters: Substring

A view of the string’s contents as a collection of characters.

var customPlaygroundQuickLook: _PlaygroundQuickLook

A custom playground Quick Look for this instance.

var isContiguousUTF8: Bool

Returns whether this string is capable of providing access to validly-encoded UTF-8 contents in contiguous memory in O(1) time.

### Instance Methods

func filter((Substring.Element) throws -> Bool) rethrows -> String

func makeContiguousUTF8()

If this string is not contiguous, make it so. If this mutates the substring, it will invalidate any pre-existing indices.

func replaceSubrange(Range&lt;Substring.Index>, with: Substring)

func withMutableCharacters&lt;R>((inout Substring) -> R) -> R

Applies the given closure to a mutable view of the string’s characters.

func withUTF8&lt;R>((UnsafeBufferPointer&lt;UInt8>) throws -> R) rethrows -> R

Runs `body` over the content of this substring in contiguous memory. If this substring is not contiguous, this will first make it contiguous, which will also speed up subsequent access. If this mutates the substring, it will invalidate any pre-existing indices.

### Type Aliases

typealias CharacterView

A view of a string’s contents as a collection of characters.

typealias Output

### Default Implementations

BidirectionalCollection Implementations

Collection Implementations

Comparable Implementations

CustomDebugStringConvertible Implementations

CustomReflectable Implementations

CustomStringConvertible Implementations

CustomTestStringConvertible Implementations

Equatable Implementations

ExpressibleByExtendedGraphemeClusterLiteral Implementations

ExpressibleByStringInterpolation Implementations

ExpressibleByStringLiteral Implementations

ExpressibleByUnicodeScalarLiteral Implementations

Hashable Implementations

LosslessStringConvertible Implementations

RangeReplaceableCollection Implementations

RegexComponent Implementations

Sequence Implementations

StringProtocol Implementations

TextOutputStream Implementations

TextOutputStreamable Implementations

## Relationships

### Conforms To

- BidirectionalCollection
- Collection
- Comparable
- Copyable
- CustomDebugStringConvertible
- CustomReflectable
- CustomStringConvertible
- CustomTestStringConvertible
- Equatable
- ExpressibleByExtendedGraphemeClusterLiteral
- ExpressibleByStringInterpolation
- ExpressibleByStringLiteral
- ExpressibleByUnicodeScalarLiteral
- Hashable
- LosslessStringConvertible
- RangeReplaceableCollection
- RegexComponent
- Sendable
- Sequence
- StringProtocol
- TextOutputStream
- TextOutputStreamable

## See Also

### Related String Types

protocol StringProtocol

A type that can represent a string as a collection of characters.

struct Index

A position of a character or code unit in a string.

struct UnicodeScalarView

A view of a string’s contents as a collection of Unicode scalar values.

struct UTF16View

A view of a string’s contents as a collection of UTF-16 code units.

struct UTF8View

A view of a string’s contents as a collection of UTF-8 code units.

struct Iterator

A type that provides the collection’s iteration interface and encapsulates its iteration state.

struct Encoding

