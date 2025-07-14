

- Foundation
-  NSMutableString 

Class

# NSMutableString

A dynamic plain-text Unicode string object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSMutableString
```

## Overview

In Swift, you can use this type instead of a String in cases that require reference semantics.

The `NSMutableString` class declares the programmatic interface to an object that manages a mutable string—that is, a string whose contents can be edited—that conceptually represents an array of Unicode characters. To construct and manage an immutable string—or a string that cannot be changed after it has been created—use an object of the NSString class.

The `NSMutableString` class adds one primitive method—replaceCharacters(in:with:)—to the basic string-handling behavior inherited from `NSString`. All other methods that modify a string work through this method. For example, insert(_:at:) simply replaces the characters in a range of `0` length, while deleteCharacters(in:) replaces the characters in a given range with no characters.

NSMutableString is “toll-free bridged” with its Core Foundation counterpart, CFMutableString. See Toll-Free Bridging for more information.

## Topics

### Creating and Initializing a Mutable String

init(capacity: Int)

Returns an `NSMutableString` object initialized with initial storage for a given number of characters,

### Modifying a String

func append(String)

Adds to the end of the receiver the characters of a given string.

func applyTransform(StringTransform, reverse: Bool, range: NSRange, updatedRange: NSRangePointer?) -> Bool

Transliterates the receiver by applying a specified ICU string transform.

func deleteCharacters(in: NSRange)

Removes from the receiver the characters in a given range.

func insert(String, at: Int)

Inserts into the receiver the characters of a given string at a given location.

func replaceCharacters(in: NSRange, with: String)

Replaces the characters from `range` with those in `aString`.

func replaceOccurrences(of: String, with: String, options: NSString.CompareOptions, range: NSRange) -> Int

Replaces all occurrences of a given string in a given range with another given string, returning the number of replacements.

func setString(String)

Replaces the characters of the receiver with those in a given string.

### Constants

String Transformations

These constants specify transforms used by the applyTransform(_:reverse:range:updatedRange:) method.

### Instance Methods

func appendFormat(NSString, any CVarArg...)

## Relationships

### Inherits From

- NSString

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- ExpressibleByExtendedGraphemeClusterLiteral
- ExpressibleByStringLiteral
- ExpressibleByUnicodeScalarLiteral
- Hashable
- NSCoding
- NSCopying
- NSItemProviderReading
- NSItemProviderWriting
- NSMutableCopying
- NSObjectProtocol
- NSSecureCoding

