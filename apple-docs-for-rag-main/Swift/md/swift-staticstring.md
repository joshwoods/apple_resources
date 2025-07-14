

- Swift
-  StaticString 

Structure

# StaticString

A string type designed to represent text that is known at compile time.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct StaticString
```

## Overview

Instances of the `StaticString` type are immutable.

`StaticString` provides only low-level access to its contents, unlike Swift’s more commonly used `String` type. A static string can use either of the following as its storage:

- a pointer to a null-terminated sequence of UTF-8 code units:

  ```
  let emoji: StaticString = "\u{1F600}"
  emoji.hasPointerRepresentation  //-> true
  emoji.isASCII                   //-> false
  emoji.unicodeScalar             //-> Fatal error!
  emoji.utf8CodeUnitCount         //-> 4
  emoji.utf8Start[0]              //-> 0xF0
  emoji.utf8Start[1]              //-> 0x9F
  emoji.utf8Start[2]              //-> 0x98
  emoji.utf8Start[3]              //-> 0x80
  emoji.utf8Start[4]              //-> 0x00
  ```

- a single Unicode scalar value, under very limited circumstances:

  ```
  struct MyStaticScalar: ExpressibleByUnicodeScalarLiteral {
      typealias UnicodeScalarLiteralType = StaticString
      let value: StaticString
      init(unicodeScalarLiteral value: StaticString) {
          self.value = value
      }
  }

  let emoji: StaticString = MyStaticScalar("\u{1F600}").value
  emoji.hasPointerRepresentation  //-> false
  emoji.isASCII                   //-> false
  emoji.unicodeScalar.value       //-> 0x1F600
  emoji.utf8CodeUnitCount         //-> Fatal error!
  emoji.utf8Start                 //-> Fatal error!
  ```

You can use the `withUTF8Buffer(_:)` method to access a static string’s contents, regardless of which representation the static string uses.

```
emoji.withUTF8Buffer { utf8 in
    utf8.count  //-> 4
    utf8[0]     //-> 0xF0
    utf8[1]     //-> 0x9F
    utf8[2]     //-> 0x98
    utf8[3]     //-> 0x80
    utf8[4]     //-> Fatal error!
}
```

## Topics

### Initializers

init()

Creates an empty static string.

### Instance Properties

var hasPointerRepresentation: Bool

A Boolean value that indicates whether the static string stores a pointer to a null-terminated sequence of UTF-8 code units.

var isASCII: Bool

A Boolean value that indicates whether the static string represents only ASCII code units (or an ASCII scalar value).

var unicodeScalar: Unicode.Scalar

A single Unicode scalar value.

var utf8CodeUnitCount: Int

The number of UTF-8 code units (excluding the null terminator).

var utf8Start: UnsafePointer&lt;UInt8>

A pointer to a null-terminated sequence of UTF-8 code units.

### Instance Methods

func withUTF8Buffer&lt;R>((UnsafeBufferPointer&lt;UInt8>) -> R) -> R

Invokes the given closure with a buffer containing the static string’s UTF-8 code unit sequence (excluding the null terminator).

### Default Implementations

CustomDebugStringConvertible Implementations

CustomReflectable Implementations

CustomStringConvertible Implementations

ExpressibleByExtendedGraphemeClusterLiteral Implementations

ExpressibleByStringLiteral Implementations

ExpressibleByUnicodeScalarLiteral Implementations

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- CustomDebugStringConvertible
- CustomReflectable
- CustomStringConvertible
- ExpressibleByExtendedGraphemeClusterLiteral
- ExpressibleByStringLiteral
- ExpressibleByUnicodeScalarLiteral
- Sendable

