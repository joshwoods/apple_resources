

- Foundation
-  NSCharacterSet 

Class

# NSCharacterSet

An object representing a fixed set of Unicode character values for use in search operations.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSCharacterSet
```

## Overview

In Swift, this bridges to a CharacterSet; use NSCharacterSet when you need reference semantics or other Foundation-specific behavior.

An `NSCharacterSet` object represents a set of Unicode-compliant characters. `NSString` and `NSScanner` objects use `NSCharacterSet` objects to group characters together for searching operations, so that they can find any of a particular set of characters during a search. The cluster’s two public classes, `NSCharacterSet` and NSMutableCharacterSet, declare the programmatic interface for static and dynamic character sets, respectively.

The objects you create using these classes are referred to as character set objects (and when no confusion will result, merely as character sets). Because of the nature of class clusters, character set objects aren’t actual instances of the `NSCharacterSet` or `NSMutableCharacterSet` classes but of one of their private subclasses. Although a character set object’s class is private, its interface is public, as declared by these abstract superclasses, `NSCharacterSet` and `NSMutableCharacterSet`. The character set classes adopt the `NSCopying` and `NSMutableCopying` protocols, making it convenient to convert a character set of one type to the other.

The `NSCharacterSet` class declares the programmatic interface for an object that manages a set of Unicode characters (see the NSString class cluster specification for information on Unicode). `NSCharacterSet`’s principal primitive method, characterIsMember(_:), provides the basis for all other instance methods in its interface. A subclass of `NSCharacterSet` needs only to implement this method, plus mutableCopy(with:), for proper behavior. For optimal performance, a subclass should also override bitmapRepresentation, which otherwise works by invoking characterIsMember(_:) for every possible Unicode value.

`NSCharacterSet` is “toll-free bridged” with its Core Foundation counterpart, CFCharacterSet. See Toll-Free Bridging for more information on toll-free bridging.

Important

The Swift overlay to the Foundation framework provides the CharacterSet structure, which bridges to the NSCharacterSet class and its mutable subclass, NSMutableCharacterSet. For more information about value types, see Working with Cocoa Frameworks in Using Swift with Cocoa and Objective-C (Swift 4.1).

## Topics

### Getting Standard Character Sets

class var alphanumerics: CharacterSet

A character set containing the characters in Unicode General Categories L\*, M\*, and N\*.

class var capitalizedLetters: CharacterSet

A character set containing the characters in Unicode General Category Lt.

class var controlCharacters: CharacterSet

A character set containing the characters in Unicode General Category Cc and Cf.

class var decimalDigits: CharacterSet

A character set containing the characters in the category of Decimal Numbers.

class var decomposables: CharacterSet

A character set containing individual Unicode characters that can also be represented as composed character sequences (such as for letters with accents), by the definition of “standard decomposition” in version 3.2 of the Unicode character encoding standard.

class var illegalCharacters: CharacterSet

A character set containing values in the category of Non-Characters or that have not yet been defined in version 3.2 of the Unicode standard.

class var letters: CharacterSet

A character set containing the characters in Unicode General Category L\* & M\*.

class var lowercaseLetters: CharacterSet

A character set containing the characters in Unicode General Category Ll.

class var newlines: CharacterSet

A character set containing the newline characters (`U+000A` ~ `U+000D`, `U+0085`, `U+2028`, and `U+2029`).

class var nonBaseCharacters: CharacterSet

A character set containing the characters in Unicode General Category M\*.

class var punctuationCharacters: CharacterSet

A character set containing the characters in Unicode General Category P\*.

class var symbols: CharacterSet

A character set containing the characters in Unicode General Category S\*.

class var uppercaseLetters: CharacterSet

A character set containing the characters in Unicode General Category Lu and Lt.

class var whitespacesAndNewlines: CharacterSet

A character set containing characters in Unicode General Category Z\*, `U+000A` ~ `U+000D`, and `U+0085`.

class var whitespaces: CharacterSet

A character set containing the characters in Unicode General Category Zs and `CHARACTER TABULATION` (`U+0009`).

### Getting Character Sets for URL Encoding

class var urlFragmentAllowed: CharacterSet

Returns the character set for characters allowed in a fragment URL component.

class var urlHostAllowed: CharacterSet

Returns the character set for characters allowed in a host URL subcomponent.

class var urlPasswordAllowed: CharacterSet

Returns the character set for characters allowed in a password URL subcomponent.

class var urlPathAllowed: CharacterSet

Returns the character set for characters allowed in a path URL component.

class var urlQueryAllowed: CharacterSet

Returns the character set for characters allowed in a query URL component.

class var urlUserAllowed: CharacterSet

Returns the character set for characters allowed in a user URL subcomponent.

### Creating a Custom Character Set

init(coder: NSCoder)

init(charactersIn: String)

Returns a character set containing the characters in a given string.

init(range: NSRange)

Returns a character set containing characters with Unicode values in a given range.

NSOpenStepUnicodeReservedBase

Specifies lower bound for a Unicode character range reserved for Apple’s corporate use.

### Creating and Managing Character Sets as Bitmap Representations

init(bitmapRepresentation: Data)

Returns a character set containing characters determined by a given bitmap representation.

init?(contentsOfFile: String)

Returns a character set read from the bitmap representation stored in the file a given path.

var bitmapRepresentation: Data

An `NSData` object encoding the receiver in binary format.

### Inverting a Character Set

var inverted: CharacterSet

A character set containing only characters that don’t exist in the receiver.

### Testing Set Membership

func characterIsMember(unichar) -> Bool

Returns a Boolean value that indicates whether a given character is in the receiver.

func hasMemberInPlane(UInt8) -> Bool

Returns a Boolean value that indicates whether the receiver has at least one member in a given character plane.

func isSuperset(of: CharacterSet) -> Bool

Returns a Boolean value that indicates whether the receiver is a superset of another given character set.

func longCharacterIsMember(UTF32Char) -> Bool

Returns a Boolean value that indicates whether a given long character is a member of the receiver.

## Relationships

### Inherits From

- NSObject

### Inherited By

- NSMutableCharacterSet

### Conforms To

- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSMutableCopying
- NSObjectProtocol
- NSSecureCoding

