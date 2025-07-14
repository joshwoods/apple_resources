

- Foundation
-  NSMutableCharacterSet 

Class

# NSMutableCharacterSet

An object representing a mutable set of Unicode character values for use in search operations.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSMutableCharacterSet
```

## Overview

In Swift, this object bridges to CharacterSet; use NSMutableCharacterSet when you need reference semantics or other Foundation-specific behavior.

The `NSMutableCharacterSet` class declares the programmatic interface to objects that manage a modifiable set of Unicode characters. You can add or remove characters from a mutable character set as numeric values in `NSRange` structures or as character values in strings, combine character sets by union or intersection, and invert a character set.

Mutable character sets are less efficient to use than immutable character sets. If you don’t need to change a character set after creating it, create an immutable copy with `copy` and use that.

`NSMutableCharacterSet` defines no primitive methods. Subclasses must implement all methods declared by this class in addition to the primitives of NSCharacterSet. They must also implement mutableCopy(with:).

`NSMutableCharacterSet` is “toll-free bridged” with its Core Foundation counterpart, CFMutableCharacterSet. See Toll-Free Bridging for more information.

Important

The Swift overlay to the Foundation framework provides the CharacterSet structure, which bridges to the NSMutableCharacterSet class and its immutable superclass, NSCharacterSet. For more information about value types, see Working with Cocoa Frameworks in Using Swift with Cocoa and Objective-C (Swift 4.1).

## Topics

### Getting Standard Character Sets

class func alphanumeric() -> NSMutableCharacterSet

Returns a character set containing the characters in Unicode General Categories L\*, M\*, and N\*.

class func capitalizedLetter() -> NSMutableCharacterSet

Returns a character set containing the characters in Unicode General Category Lt.

class func control() -> NSMutableCharacterSet

Returns a character set containing the characters in Unicode General Category Cc and Cf.

class func decimalDigit() -> NSMutableCharacterSet

Returns a character set containing the characters in the category of decimal numbers.

class func decomposable() -> NSMutableCharacterSet

Returns a character set containing individual Unicode characters that can also be represented as composed character sequences (such as for letters with accents), by the definition of “standard decomposition” in version 3.2 of the Unicode character encoding standard.

class func illegal() -> NSMutableCharacterSet

Returns a character set containing values in the category of Non-Characters or that have not yet been defined in version 3.2 of the Unicode standard.

class func letter() -> NSMutableCharacterSet

Returns a character set containing the characters in Unicode General Category L\* & M\*.

class func lowercaseLetter() -> NSMutableCharacterSet

Returns a character set containing the characters in Unicode General Category Ll.

class func newline() -> NSMutableCharacterSet

Returns a character set containing the newline characters (`U+000A` ~ `U+000D`, `U+0085`, `U+2028`, and `U+2029`).

class func nonBase() -> NSMutableCharacterSet

Returns a character set containing the characters in Unicode General Category M\*.

class func punctuation() -> NSMutableCharacterSet

Returns a character set containing the characters in Unicode General Category P\*.

class func symbol() -> NSMutableCharacterSet

Returns a character set containing the characters in Unicode General Category S\*.

class func uppercaseLetter() -> NSMutableCharacterSet

Returns a character set containing the characters in Unicode General Category Lu and Lt.

class func whitespaceAndNewline() -> NSMutableCharacterSet

Returns a character set containing characters in Unicode General Category Z\*, `U+000A` ~ `U+000D`, and `U+0085`.

class func whitespace() -> NSMutableCharacterSet

Returns a character set containing the characters in Unicode General Category Zs and `CHARACTER TABULATION` (`U+0009`).

### Creating Custom Character Sets

init(charactersIn: String)

Returns a character set containing the characters in a given string.

init(range: NSRange)

Returns a character set containing characters with Unicode values in a given range.

init(bitmapRepresentation: Data)

Returns a character set containing characters determined by a given bitmap representation.

init?(contentsOfFile: String)

Returns a character set read from the bitmap representation stored in the file a given path.

### Adding and Removing Characters

func addCharacters(in: NSRange)

Adds to the receiver the characters whose Unicode values are in a given range.

func removeCharacters(in: NSRange)

Removes from the receiver the characters whose Unicode values are in a given range.

func addCharacters(in: String)

Adds to the receiver the characters in a given string.

func removeCharacters(in: String)

Removes from the receiver the characters in a given string.

### Combining Character Sets

func formIntersection(with: CharacterSet)

Modifies the receiver so it contains only characters that exist in both the receiver and another set.

func formUnion(with: CharacterSet)

Modifies the receiver so it contains all characters that exist in either the receiver or another set.

### Inverting a Character Set

func invert()

Replaces all the characters in the receiver with all the characters it didn’t previously contain.

## Relationships

### Inherits From

- NSCharacterSet

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSMutableCopying
- NSObjectProtocol
- NSSecureCoding

