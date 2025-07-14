

- Foundation
-  Strings and Text 

API Collection

# Strings and Text

Create and process strings of Unicode characters, use regular expressions to find patterns, and perform natural language analysis of text.

## Topics

### Strings

@frozen struct String

A Unicode string value that is a collection of characters.

String Encodings

Constants for encoding standards used when converting raw data to and from string representations.

### Strings with Metadata

struct AttributedString

A value type for a string with associated attributes for portions of its text.

struct AttributedSubstring

A portion of an attributed string.

Attributed String Supporting Types

Types that the attributed string, attributed substring, and helper types extend or conform to, for sharing common functionality.

class NSAttributedString

A string of text that manages data, layout, and stylistic information for ranges of characters to support rendering.

class NSMutableAttributedString

A mutable string with associated attributes (such as visual style, hyperlinks, or accessibility data) for portions of its text.

### Characters

struct CharacterSet

A set of Unicode character values for use in search operations.

typealias UnicodeScalar = Unicode.Scalar

### Pattern Matching

class Scanner

A string parser that scans for substrings or characters in a character set, and for numeric values from decimal, hexadecimal, and floating-point representations.

class NSRegularExpression

An immutable representation of a compiled regular expression that you apply to Unicode strings.

class NSDataDetector

A specialized regular expression object that matches natural language text for predefined data patterns.

class NSTextCheckingResult

An occurrence of textual content found during the analysis of a block of text, such as when matching a regular expression.

let NSNotFound: Int

A value indicating that a requested item couldn’t be found or doesn’t exist.

### Spelling and Grammar

class NSSpellServer

A server that your app uses to provide a spell checker service to other apps running in the system.

protocol NSSpellServerDelegate

The optional methods implemented by the delegate of a spell server.

### Localization

struct Locale

Information about linguistic, cultural, and technological conventions for use in formatting data for presentation.

class NSOrthography

A description of the linguistic content of natural language text, typically used for spelling and grammar checking.

func NSLocalizedString(String, tableName: String?, bundle: Bundle, value: String, comment: String) -> String

Returns a localized string from a table that Xcode generates for you when exporting localizations.

struct LocalizedStringResource

A reference to a localizable string, accessible from another process.

protocol CustomLocalizedStringResourceConvertible

A type that provides an out-of-process localizable description.

struct URLResource

A resource located at a particular file URL within a bundle.

### Deprecated

class NSLinguisticTagger

Analyze natural language text to tag part of speech and lexical class, identify names, perform lemmatization, and determine the language and script.

Deprecated

Deprecated String Encodings

## See Also

### Fundamentals

Numbers, Data, and Basic Values

Work with primitive values and other fundamental types used throughout Cocoa.

Collections

Use arrays, dictionaries, sets, and specialized collections to store and iterate groups of objects or values.

Dates and Times

Compare dates and times, and perform calendar and time zone calculations.

Units and Measurement

Label numeric quantities with physical dimensions to allow locale-aware formatting and conversion between related units.

Data Formatting

Convert numbers, dates, measurements, and other values to and from locale-aware string representations.

Filters and Sorting

Use predicates, expressions, and sort descriptors to examine elements in collections and other services.

