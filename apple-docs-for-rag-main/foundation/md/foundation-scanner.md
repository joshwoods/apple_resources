

- Foundation
-  Scanner 

Class

# Scanner

A string parser that scans for substrings or characters in a character set, and for numeric values from decimal, hexadecimal, and floating-point representations.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class Scanner
```

## Overview

A Scanner object interprets and converts the characters of a String into number and string values. You assign the scanner’s string when you create the scanner, and the scanner progresses through the characters of that string from beginning to end as you request items.

Because of the nature of class clusters, a scanner object isn’t an actual instance of the Scanner class, but is one of its private subclasses. Although a scanner object’s class is private, its interface is public, as declared by this abstract superclass, Scanner. The objects you create using this class are referred to as scanner objects (and when no confusion will result, merely as scanners).

To set a Scanner object to ignore a set of characters as it scans the string, use the charactersToBeSkipped property. Characters in the skip set are skipped over before the target is scanned. The default set of characters to skip is the whitespace and newline character set.

To retrieve the unscanned remainder of the string, use `scanner.string.substring(from: scanner.scanLocation)`.

## Topics

### Creating a Scanner

class func localizedScanner(with: String) -> Any

Returns an `NSScanner` object that scans a given string according to the user’s default locale.

init(string: String)

Returns an `NSScanner` object initialized to scan a given string.

### Getting a Scanner’s String

var string: String

The string the scanner will scan.

### Configuring a Scanner

var scanLocation: Int

The character position at which the receiver will begin its next scanning operation.

Deprecated

var caseSensitive: Bool

Flag that indicates whether the receiver distinguishes case in the characters it scans.

var charactersToBeSkipped: CharacterSet?

Character set containing the characters the scanner ignores when looking for a scannable element.

var locale: Any?

The locale to use when scanning.

### Scanning Characters and Strings

func scanCharacters(from: CharacterSet, into: AutoreleasingUnsafeMutablePointer&lt;NSString?>?) -> Bool

Scans the string as long as characters from a given character set are encountered, accumulating characters into a string that’s returned by reference.

Deprecated

func scanUpToCharacters(from: CharacterSet, into: AutoreleasingUnsafeMutablePointer&lt;NSString?>?) -> Bool

Scans the string until a character from a given character set is encountered, accumulating characters into a string that’s returned by reference.

Deprecated

func scanString(String, into: AutoreleasingUnsafeMutablePointer&lt;NSString?>?) -> Bool

Scans a given string, returning an equivalent string object by reference if a match is found.

Deprecated

func scanUpTo(String, into: AutoreleasingUnsafeMutablePointer&lt;NSString?>?) -> Bool

Scans the string until a given string is encountered, accumulating characters into a string that’s returned by reference.

Deprecated

### Scanning Numeric Values

func scanDecimal(UnsafeMutablePointer&lt;Decimal>?) -> Bool

Scans for an `NSDecimal` value, returning a found value by reference.

Deprecated

func scanDouble(UnsafeMutablePointer&lt;Double>?) -> Bool

Scans for a double value, returning a found value by reference.

Deprecated

func scanFloat(UnsafeMutablePointer&lt;Float>?) -> Bool

Scans for a float value, returning a found value by reference.

Deprecated

func scanHexDouble(UnsafeMutablePointer&lt;Double>?) -> Bool

Scans for a double value from a hexadecimal representation, returning a found value by reference.

func scanHexFloat(UnsafeMutablePointer&lt;Float>?) -> Bool

Scans for a double value from a hexadecimal representation, returning a found value by reference.

func scanHexInt32(UnsafeMutablePointer&lt;UInt32>?) -> Bool

Scans for an unsigned value from a hexadecimal representation, returning a found value by reference.

Deprecated

func scanHexInt64(UnsafeMutablePointer&lt;UInt64>?) -> Bool

Scans for a long long value from a hexadecimal representation, returning a found value by reference.

func scanInt(UnsafeMutablePointer&lt;Int>?) -> Bool

Scans for an NSInteger value from a decimal representation, returning a found value by reference

func scanInt32(UnsafeMutablePointer&lt;Int32>?) -> Bool

Scans for an int value from a decimal representation, returning a found value by reference.

Deprecated

func scanInt64(UnsafeMutablePointer&lt;Int64>?) -> Bool

Scans for a long long value from a decimal representation, returning a found value by reference.

func scanUnsignedLongLong(UnsafeMutablePointer&lt;UInt64>?) -> Bool

Scans for an unsigned long long value from a decimal representation, returning a found value by reference.

### Monitoring Scanner Progress

var isAtEnd: Bool

Flag that indicates whether the receiver has exhausted all significant characters.

### Instance Properties

var currentIndex: String.Index

### Instance Methods

func scanCharacter() -> Character?

func scanCharacters(from: CharacterSet) -> String?

func scanDecimal() -> Decimal?

func scanDouble(representation: Scanner.NumberRepresentation) -> Double?

func scanFloat(representation: Scanner.NumberRepresentation) -> Float?

func scanInt(representation: Scanner.NumberRepresentation) -> Int?

func scanInt32(representation: Scanner.NumberRepresentation) -> Int32?

func scanInt64(representation: Scanner.NumberRepresentation) -> Int64?

func scanString(String) -> String?

func scanUInt64(representation: Scanner.NumberRepresentation) -> UInt64?

func scanUpToCharacters(from: CharacterSet) -> String?

func scanUpToString(String) -> String?

### Enumerations

enum NumberRepresentation

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Pattern Matching

class NSRegularExpression

An immutable representation of a compiled regular expression that you apply to Unicode strings.

class NSDataDetector

A specialized regular expression object that matches natural language text for predefined data patterns.

class NSTextCheckingResult

An occurrence of textual content found during the analysis of a block of text, such as when matching a regular expression.

let NSNotFound: Int

A value indicating that a requested item couldn’t be found or doesn’t exist.

