

- Swift
-  Regex 

Structure

# Regex

A regular expression.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct Regex
```

## Overview

Regular expressions are a concise way of describing a pattern, which can help you match or extract portions of a string. You can create a `Regex` instance using regular expression syntax, either in a regex literal or a string.

```
// 'keyAndValue' is created using a regex literal
let keyAndValue = /(.+?): (.+)/
// 'simpleDigits' is created from a pattern in a string
let simpleDigits = try Regex("[0-9]+")
```

You can use a `Regex` to search for a pattern in a string or substring. Call `contains(_:)` to check for the presence of a pattern, or `firstMatch(of:)` or `matches(of:)` to find matches.

```
let setting = "color: 161 103 230"
if setting.contains(simpleDigits) {
    print("'\(setting)' contains some digits.")
}
// Prints "'color: 161 103 230' contains some digits."
```

When you find a match, the resulting Regex.Match type includes an output property that contains the matched substring along with any captures:

```
if let match = setting.firstMatch(of: keyAndValue) {
    print("Key: \(match.1)")
    print("Value: \(match.2)")
}
// Key: color
// Value: 161 103 230
```

When you import the `RegexBuilder` module, you can also create `Regex` instances using a clear and flexible declarative syntax. Using this style, you can combine, capture, and transform regexes, `RegexBuilder` types, and custom parsers.

Note

Prior to Swift 6, you might need to write `#/myregex/#` instead of `/myregex/` when you make a regular expression using a literal. For more information, see Regular Expression Literals in *The Swift Programming Language*.

## Topics

### Structures

struct Match

The result of matching a regular expression against a string.

### Initializers

init(() -> some RegexComponent&lt;Output>)

Creates a regular expression using a RegexBuilder closure.

init(String) throws

Creates a regular expression from the given string, using a dynamic capture list.

init&lt;OtherOutput>(Regex&lt;OtherOutput>)

Creates a regular expression with a dynamic capture list from the given regular expression.

init?(Regex&lt;AnyRegexOutput>, as: Output.Type)

Creates a regular expression with a strongly-typed capture list from the given regular expression.

init(String, as: Output.Type) throws

Creates a regular expression from the given string, using the specified capture type.

init(verbatim: String)

Creates a regular expression that matches the given string exactly, as though every metacharacter in it was escaped.

### Instance Properties

var regex: Regex&lt;Output>

The regular expression represented by this component.

### Instance Methods

func anchorsMatchLineEndings(Bool) -> Regex&lt;Regex&lt;Output>.RegexOutput>

Returns a regular expression where the start and end of input anchors (`^` and `$`) also match against the start and end of a line.

func asciiOnlyCharacterClasses(Bool) -> Regex&lt;Regex&lt;Output>.RegexOutput>

Returns a regular expression that matches only ASCII characters when matching character classes.

func asciiOnlyDigits(Bool) -> Regex&lt;Regex&lt;Output>.RegexOutput>

Returns a regular expression that matches only ASCII characters as digits.

func asciiOnlyWhitespace(Bool) -> Regex&lt;Regex&lt;Output>.RegexOutput>

Returns a regular expression that matches only ASCII characters as space characters.

func asciiOnlyWordCharacters(Bool) -> Regex&lt;Regex&lt;Output>.RegexOutput>

Returns a regular expression that matches only ASCII characters as word characters.

func contains(captureNamed: String) -> Bool

Returns a Boolean value indicating whether a named capture with the given name exists.

func dotMatchesNewlines(Bool) -> Regex&lt;Regex&lt;Output>.RegexOutput>

Returns a regular expression where the “any” metacharacter (`.`) also matches against the start and end of a line.

func firstMatch(in: Substring) throws -> Regex&lt;Output>.Match?

Returns the first match for this regex found in the given substring.

func firstMatch(in: String) throws -> Regex&lt;Output>.Match?

Returns the first match for this regex found in the given string.

func ignoresCase(Bool) -> Regex&lt;Regex&lt;Output>.RegexOutput>

Returns a regular expression that ignores case when matching.

func matchingSemantics(RegexSemanticLevel) -> Regex&lt;Regex&lt;Output>.RegexOutput>

Returns a regular expression that matches with the specified semantic level.

func prefixMatch(in: Substring) throws -> Regex&lt;Output>.Match?

Returns a match if this regex matches the given substring at its start.

func prefixMatch(in: String) throws -> Regex&lt;Output>.Match?

Returns a match if this regex matches the given string at its start.

func repetitionBehavior(RegexRepetitionBehavior) -> Regex&lt;Regex&lt;Output>.RegexOutput>

Returns a regular expression where quantifiers use the specified behavior by default.

func wholeMatch(in: Substring) throws -> Regex&lt;Output>.Match?

Returns a match if this regex matches the given substring in its entirety.

func wholeMatch(in: String) throws -> Regex&lt;Output>.Match?

Returns a match if this regex matches the given string in its entirety.

func wordBoundaryKind(RegexWordBoundaryKind) -> Regex&lt;Regex&lt;Output>.RegexOutput>

Returns a regular expression that uses the specified word boundary algorithm.

### Type Aliases

typealias RegexOutput

The output type for this regular expression.

## Relationships

### Conforms To

- RegexComponent

## See Also

### Regular Expressions

struct RegexRepetitionBehavior

Specifies how much to attempt to match when using a quantifier.

struct RegexSemanticLevel

A semantic level to use during regex matching.

struct RegexWordBoundaryKind

A word boundary algorithm to use during regex matching.

struct AnyRegexOutput

The type-erased, dynamic output of a regular expression match.

protocol RegexComponent

A type that represents a regular expression.

protocol CustomConsumingRegexComponent

