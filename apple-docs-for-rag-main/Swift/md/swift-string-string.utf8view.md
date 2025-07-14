

- Swift
- String
-  String.UTF8View 

Structure

# String.UTF8View

A view of a string’s contents as a collection of UTF-8 code units.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct UTF8View
```

## Overview

You can access a string’s view of UTF-8 code units by using its `utf8` property. A string’s UTF-8 view encodes the string’s Unicode scalar values as 8-bit integers.

```
let flowers = "Flowers 💐"
for v in flowers.utf8 {
    print(v)
}
// 70
// 108
// 111
// 119
// 101
// 114
// 115
// 32
// 240
// 159
// 146
// 144
```

A string’s Unicode scalar values can be up to 21 bits in length. To represent those scalar values using 8-bit integers, more than one UTF-8 code unit is often required.

```
let flowermoji = "💐"
for v in flowermoji.unicodeScalars {
    print(v, v.value)
}
// 💐 128144

for v in flowermoji.utf8 {
    print(v)
}
// 240
// 159
// 146
// 144
```

In the encoded representation of a Unicode scalar value, each UTF-8 code unit after the first is called a *continuation byte*.

# UTF8View Elements Match Encoded C Strings

Swift streamlines interoperation with C string APIs by letting you pass a `String` instance to a function as an `Int8` or `UInt8` pointer. When you call a C function using a `String`, Swift automatically creates a buffer of UTF-8 code units and passes a pointer to that buffer. The code units of that buffer match the code units in the string’s `utf8` view.

The following example uses the C `strncmp` function to compare the beginning of two Swift strings. The `strncmp` function takes two `const char*` pointers and an integer specifying the number of characters to compare. Because the strings are identical up to the 14th character, comparing only those characters results in a return value of `0`.

```
let s1 = "They call me 'Bell'"
let s2 = "They call me 'Stacey'"

print(strncmp(s1, s2, 14))
// Prints "0"
print(String(s1.utf8.prefix(14))!)
// Prints "They call me '"
```

Extending the compared character count to 15 includes the differing characters, so a nonzero result is returned.

```
print(strncmp(s1, s2, 15))
// Prints "-17"
print(String(s1.utf8.prefix(15))!)
// Prints "They call me 'B"
```

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

Sequence Implementations

## Relationships

### Conforms To

- BidirectionalCollection
- Collection
- Copyable
- CustomDebugStringConvertible
- CustomReflectable
- CustomStringConvertible
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

struct UnicodeScalarView

A view of a string’s contents as a collection of Unicode scalar values.

struct UTF16View

A view of a string’s contents as a collection of UTF-16 code units.

struct Iterator

A type that provides the collection’s iteration interface and encapsulates its iteration state.

struct Encoding

