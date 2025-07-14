

- Foundation
-  NSTextCheckingResult 

Class

# NSTextCheckingResult

An occurrence of textual content found during the analysis of a block of text, such as when matching a regular expression.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSTextCheckingResult
```

## Overview

On both iOS and macOS, instances of NSTextCheckingResult are returned by the NSRegularExpression class and the NSDataDetector class to indicate the discovery of content. In those cases, what is found may be a match for a regular expression or a date, address, phone number, and so on. In macOS, instances of `NSTextCheckingResult` are returned by the NSSpellChecker object to describe the results of spelling, grammar, or text-substitution actions.

## Topics

### Text Checking Type Range and Type

var range: NSRange

Returns the range of the result that the receiver represents.

var resultType: NSTextCheckingResult.CheckingType

Returns the text checking result type that the receiver represents.

var numberOfRanges: Int

Returns the number of ranges.

func range(at: Int) -> NSRange

Returns the result type that the range represents.

### Text Checking Results for Text Replacement

class func replacementCheckingResult(range: NSRange, replacementString: String) -> NSTextCheckingResult

Creates and returns a text checking result with the specified replacement string.

var replacementString: String?

A replacement string from one of a number of replacement checking results.

### Text Checking Results for Regular Expressions

class func regularExpressionCheckingResult(ranges: NSRangePointer, count: Int, regularExpression: NSRegularExpression) -> NSTextCheckingResult

Creates and returns a type checking result with the specified regular expression data.

var regularExpression: NSRegularExpression?

The regular expression of a type checking result.

### Text Checking Result Components

var components: [NSTextCheckingKey : String]?

A dictionary containing the components of a type checking result.

### Text Checking Results for URLs

class func linkCheckingResult(range: NSRange, url: URL) -> NSTextCheckingResult

Creates and returns a text checking result with the specified URL.

var url: URL?

The URL of a type checking result.

### Text Checking Results for Addresses

class func addressCheckingResult(range: NSRange, components: [NSTextCheckingKey : String]) -> NSTextCheckingResult

Creates and returns a text checking result with the specified address components.

var addressComponents: [NSTextCheckingKey : String]?

The address dictionary of a type checking result.

### Text Checking Results for Transit Information

class func transitInformationCheckingResult(range: NSRange, components: [NSTextCheckingKey : String]) -> NSTextCheckingResult

Creates and returns a text checking result with the specified transit information.

### Text Checking Results for Phone Numbers

class func phoneNumberCheckingResult(range: NSRange, phoneNumber: String) -> NSTextCheckingResult

Creates and returns a text checking result with the specified phone number.

var phoneNumber: String?

The phone number of a type checking result.

### Text Checking Results for Dates and Times

class func dateCheckingResult(range: NSRange, date: Date) -> NSTextCheckingResult

Creates and returns a text checking result with the specified date.

class func dateCheckingResult(range: NSRange, date: Date, timeZone: TimeZone, duration: TimeInterval) -> NSTextCheckingResult

Creates and returns a text checking result with the specified date, time zone, and duration.

var date: Date?

The date component of a type checking result.

var duration: TimeInterval

The duration component of a type checking result.

var timeZone: TimeZone?

The time zone component of a type checking result.

### Text Checking Results for Typography

class func dashCheckingResult(range: NSRange, replacementString: String) -> NSTextCheckingResult

Creates and returns a text checking result with the specified dash corrected replacement string.

class func quoteCheckingResult(range: NSRange, replacementString: String) -> NSTextCheckingResult

Creates and returns a text checking result with the specified quote-balanced replacement string.

### Text Checking Results for Spelling

class func spellCheckingResult(range: NSRange) -> NSTextCheckingResult

Creates and returns a text checking result with the range of a misspelled word.

class func correctionCheckingResult(range: NSRange, replacementString: String) -> NSTextCheckingResult

Creates and returns a text checking result after detecting a possible correction.

### Text Checking Results for Orthography

class func orthographyCheckingResult(range: NSRange, orthography: NSOrthography) -> NSTextCheckingResult

Creates and returns a text checking result with the specified orthography.

var orthography: NSOrthography?

The detected orthography of a type checking result.

### Text Checking Results for Grammar

class func grammarCheckingResult(range: NSRange, details: [[String : Any]]) -> NSTextCheckingResult

Creates and returns a text checking result with the specified array of grammatical errors.

var grammarDetails: [[String : Any]]?

The details of a located grammatical type checking result.

### Adjusting the Ranges of a Text Checking Result

func adjustingRanges(offset: Int) -> NSTextCheckingResult

Returns a new text checking result after adjusting the ranges as specified by the offset.

### Constants

Keys for Transit Components

The following constants identify the possible keys returned in the components dictionary.

Keys for Address Components

The following constants identify the possible keys returned in the addressComponents dictionary.

struct CheckingType

These constants specify the type of checking the methods should do. They are returned by resultType.

typealias NSTextCheckingTypes

Defines the types of checking that are available. These values can be combined using the C-bitwise OR operator. The system supports its own internal types, and the user can extend those types by subclassing `NSTextCheckingResult` and adding their own custom types.

struct NSTextCheckingKey

Anonymous

### Instance Properties

var alternativeStrings: [String]?

### Instance Methods

func range(withName: String) -> NSRange

### Type Methods

class func correctionCheckingResult(range: NSRange, replacementString: String, alternativeStrings: [String]) -> NSTextCheckingResult

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Pattern Matching

class Scanner

A string parser that scans for substrings or characters in a character set, and for numeric values from decimal, hexadecimal, and floating-point representations.

class NSRegularExpression

An immutable representation of a compiled regular expression that you apply to Unicode strings.

class NSDataDetector

A specialized regular expression object that matches natural language text for predefined data patterns.

let NSNotFound: Int

A value indicating that a requested item couldn’t be found or doesn’t exist.

