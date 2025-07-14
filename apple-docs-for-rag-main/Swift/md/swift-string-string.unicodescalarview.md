

- Swift
- String
-  String.UnicodeScalarView 

Structure

# String.UnicodeScalarView

A view of a string’s contents as a collection of Unicode scalar values.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct UnicodeScalarView
```

## Overview

You can access a string’s view of Unicode scalar values by using its `unicodeScalars` property. Unicode scalar values are the 21-bit codes that are the basic unit of Unicode. Each scalar value is represented by a `Unicode.Scalar` instance and is equivalent to a UTF-32 code unit.

```
let flowers = "Flowers 💐"
for v in flowers.unicodeScalars {
    print(v.value)
}
// 70
// 108
// 111
// 119
// 101
// 114
// 115
// 32
// 128144
```

Some characters that are visible in a string are made up of more than one Unicode scalar value. In that case, a string’s `unicodeScalars` view contains more elements than the string itself.

```
let flag = "🇵🇷"
for c in flag {
    print(c)
}
// 🇵🇷

for v in flag.unicodeScalars {
    print(v.value)
}
// 127477
// 127479
```

You can convert a `String.UnicodeScalarView` instance back into a string using the `String` type’s `init(_:)` initializer.

```
let favemoji = "My favorite emoji is 🎉"
if let i = favemoji.unicodeScalars.firstIndex(where: { $0.value >= 128 }) {
    let asciiPrefix = String(favemoji.unicodeScalars[..

## Topics

### Instance Properties

var customPlaygroundQuickLook: _PlaygroundQuickLook

A custom playground Quick Look for this instance.

### Default Implementations

BidirectionalCollection Implementations

Collection Implementations

CustomDebugStringConvertible Implementations

CustomReflectable Implementations

CustomStringConvertible Implementations

RangeReplaceableCollection Implementations

Sequence Implementations

## Relationships

### Conforms To

- BidirectionalCollection
- Collection
- Copyable
- CustomDebugStringConvertible
- CustomReflectable
- CustomStringConvertible
- RangeReplaceableCollection
- Sendable
- Sequence

## See Also

### Related String Types

struct Substring

A slice of a string.

protocol StringProtocol

A type that can represent a string as a collection of characters.

struct Index

A position of a character or code unit in a string.

struct UTF16View

A view of a string’s contents as a collection of UTF-16 code units.

struct UTF8View

A view of a string’s contents as a collection of UTF-8 code units.

struct Iterator

A type that provides the collection’s iteration interface and encapsulates its iteration state.

struct Encoding

