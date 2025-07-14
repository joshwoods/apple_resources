

- Foundation
-  CharacterSet 

Structure

# CharacterSet

A set of Unicode character values for use in search operations.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct CharacterSet
```

## Overview

A `CharacterSet` represents a set of Unicode-compliant characters. Foundation types use `CharacterSet` to group characters together for searching operations, so that they can find any of a particular set of characters during a search.

This type provides “copy-on-write” behavior, and is also bridged to the Objective-C `NSCharacterSet` class.

## Topics

### Getting Standard Character Sets

static var alphanumerics: CharacterSet

Returns a character set containing the characters in Unicode General Categories L\*, M\*, and N\*.

static var capitalizedLetters: CharacterSet

Returns a character set containing the characters in Unicode General Category Lt.

static var controlCharacters: CharacterSet

Returns a character set containing the characters in Unicode General Category Cc and Cf.

static var decimalDigits: CharacterSet

Returns a character set containing the characters in the category of Decimal Numbers.

static var decomposables: CharacterSet

Returns a character set containing individual Unicode characters that can also be represented as composed character sequences (such as for letters with accents), by the definition of “standard decomposition” in version 3.2 of the Unicode character encoding standard.

static var illegalCharacters: CharacterSet

Returns a character set containing values in the category of Non-Characters or that have not yet been defined in version 3.2 of the Unicode standard.

static var letters: CharacterSet

Returns a character set containing the characters in Unicode General Category L\* & M\*.

static var lowercaseLetters: CharacterSet

Returns a character set containing the characters in Unicode General Category Ll.

static var newlines: CharacterSet

Returns a character set containing the newline characters (`U+000A ~ U+000D`, `U+0085`, `U+2028`, and `U+2029`).

static var nonBaseCharacters: CharacterSet

Returns a character set containing the characters in Unicode General Category M\*.

static var punctuationCharacters: CharacterSet

Returns a character set containing the characters in Unicode General Category P\*.

static var symbols: CharacterSet

Returns a character set containing the characters in Unicode General Category S\*.

static var uppercaseLetters: CharacterSet

Returns a character set containing the characters in Unicode General Category Lu and Lt.

static var whitespaces: CharacterSet

Returns a character set containing the characters in Unicode General Category Zs and `CHARACTER TABULATION (U+0009)`.

static var whitespacesAndNewlines: CharacterSet

Returns a character set containing characters in Unicode General Category Z\*, `U+000A ~ U+000D`, and `U+0085`.

### Getting Character Sets for URL Encoding

static var urlFragmentAllowed: CharacterSet

Returns the character set for characters allowed in a fragment URL component.

static var urlHostAllowed: CharacterSet

Returns the character set for characters allowed in a host URL subcomponent.

static var urlPasswordAllowed: CharacterSet

Returns the character set for characters allowed in a password URL subcomponent.

static var urlPathAllowed: CharacterSet

Returns the character set for characters allowed in a path URL component.

static var urlQueryAllowed: CharacterSet

Returns the character set for characters allowed in a query URL component.

static var urlUserAllowed: CharacterSet

Returns the character set for characters allowed in a user URL subcomponent.

### Creating a Custom Character Set

init()

Initialize an empty instance.

### Creating and Managing Bitmap Representations

var bitmapRepresentation: Data

Returns a representation of the `CharacterSet` in binary format.

### Inverting a Character Set

func invert()

Invert the contents of the `CharacterSet`.

var inverted: CharacterSet

Returns an inverted copy of the receiver.

### Combining Character Sets

func formIntersection(CharacterSet)

Sets the value to an intersection of the `CharacterSet` with another `CharacterSet`.

func formSymmetricDifference(CharacterSet)

Sets the value to an exclusive or of the `CharacterSet` with another `CharacterSet`.

func formUnion(CharacterSet)

Sets the value to a union of the `CharacterSet` with another `CharacterSet`.

func hasMember(inPlane: UInt8) -> Bool

Returns true if the `CharacterSet` has a member in the specified plane.

func insert(charactersIn: String)

Insert the values from the specified string into the `CharacterSet`.

func intersection(CharacterSet) -> CharacterSet

Returns an intersection of the `CharacterSet` with another `CharacterSet`.

func invert()

Invert the contents of the `CharacterSet`.

func isSuperset(of: CharacterSet) -> Bool

Returns true if `self` is a superset of `other`.

func remove(charactersIn: String)

Remove the values from the specified string from the `CharacterSet`.

func subtracting(CharacterSet) -> CharacterSet

Returns a `CharacterSet` created by removing elements in `other` from `self`.

func symmetricDifference(CharacterSet) -> CharacterSet

Returns an exclusive or of the `CharacterSet` with another `CharacterSet`.

func union(CharacterSet) -> CharacterSet

Returns a union of the `CharacterSet` with another `CharacterSet`.

### Adding Characters

func insert(charactersIn: String)

Insert the values from the specified string into the `CharacterSet`.

### Removing Characters

func remove(charactersIn: String)

Remove the values from the specified string from the `CharacterSet`.

func subtracting(CharacterSet) -> CharacterSet

Returns a `CharacterSet` created by removing elements in `other` from `self`.

### Testing Set Membership

func hasMember(inPlane: UInt8) -> Bool

Returns true if the `CharacterSet` has a member in the specified plane.

func isSuperset(of: CharacterSet) -> Bool

Returns true if `self` is a superset of `other`.

### Comparing Character Sets

static func == (CharacterSet, CharacterSet) -> Bool

Returns true if the two `CharacterSet`s are equal.

### Using Reference Types

class NSCharacterSet

An object representing a fixed set of Unicode character values for use in search operations.

class NSMutableCharacterSet

An object representing a mutable set of Unicode character values for use in search operations.

### Initializers

init(bitmapRepresentation: Data)

init(charactersIn: ClosedRange&lt;Unicode.Scalar>)

init(charactersIn: String)

init(charactersIn: Range&lt;Unicode.Scalar>)

init?(contentsOfFile: String)

### Instance Methods

func contains(Unicode.Scalar) -> Bool

func insert(Unicode.Scalar) -> (inserted: Bool, memberAfterInsert: Unicode.Scalar)

func insert(charactersIn: Range&lt;Unicode.Scalar>)

func insert(charactersIn: ClosedRange&lt;Unicode.Scalar>)

func remove(Unicode.Scalar) -> Unicode.Scalar?

func remove(charactersIn: ClosedRange&lt;Unicode.Scalar>)

func remove(charactersIn: Range&lt;Unicode.Scalar>)

func subtract(CharacterSet)

func update(with: Unicode.Scalar) -> Unicode.Scalar?

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- ExpressibleByArrayLiteral
- Hashable
- ReferenceConvertible
- Sendable
- SetAlgebra

## See Also

### Characters

typealias UnicodeScalar = Unicode.Scalar

