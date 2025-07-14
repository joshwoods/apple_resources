

- Swift
-  RegexComponent 

Protocol

# RegexComponent

A type that represents a regular expression.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol RegexComponent
```

## Overview

You can use types that conform to `RegexComponent` as parameters to string searching operations and inside `RegexBuilder` closures.

## Topics

### Creating a regex component

init(CharacterClass, CharacterClass...)

Creates a character class that combines the given classes in a union.

### Getting a regex from a component

var regex: Regex&lt;Self.RegexOutput>

The regular expression represented by this component.

**Required** Default implementation provided.

### Matching substring sequences

static func anyOf&lt;S>(S) -> CharacterClass

Returns a character class that matches any Unicode scalar in the given sequence.

static func anyOf&lt;S>(S) -> CharacterClass

Returns a character class that matches any character in the given string or sequence.

static var any: CharacterClass

A character class that matches any element.

static var anyGraphemeCluster: CharacterClass

A character class that matches any single `Character`, or extended grapheme cluster, regardless of the current semantic level.

static var anyNonNewline: CharacterClass

A character class that matches any element that isn’t a newline.

static var digit: CharacterClass

A character class that matches any digit.

static var hexDigit: CharacterClass

A character class that matches any hexadecimal digit.

static var word: CharacterClass

A character class that matches any element that is a “word character”.

### Matching whitespace and line endings

static var horizontalWhitespace: CharacterClass

A character class that matches any element that is classified as horizontal whitespace.

static var newlineSequence: CharacterClass

A character class that matches any newline sequence.

static var verticalWhitespace: CharacterClass

A character class that matches any element that is classified as vertical whitespace.

static var whitespace: CharacterClass

A character class that matches any element that is classified as whitespace.

### Matching dates and times

static func date(Date.FormatStyle.DateStyle, locale: Locale, timeZone: TimeZone, calendar: Calendar?) -> Date.ParseStrategy

Creates a regex component that matches a localized date string formatted in accordance with a style, capturing it as a Foundation date.

static func date(format: Date.FormatString, locale: Locale, timeZone: TimeZone, calendar: Calendar?, twoDigitStartDate: Date) -> Self

Creates a regex component that matches a localized date string formatted in accordance with a format string, capturing it as a Foundation date.

static func dateTime(date: Date.FormatStyle.DateStyle, time: Date.FormatStyle.TimeStyle, locale: Locale, timeZone: TimeZone, calendar: Calendar?) -> Date.ParseStrategy

Creates a regex component that matches a localized date and time string, capturing it as a Foundation date.

static var iso8601: Date.ISO8601FormatStyle

A regex component that matches a default ISO 8601-formatted date string, capturing it as a Foundation date.

static func iso8601Date(timeZone: TimeZone, dateSeparator: Date.ISO8601FormatStyle.DateSeparator) -> Self

Creates a regex component that matches an ISO 8601-formatted date string, capturing it as a Foundation date in the specified time zone.

static func iso8601(timeZone: TimeZone, includingFractionalSeconds: Bool, dateSeparator: Date.ISO8601FormatStyle.DateSeparator, dateTimeSeparator: Date.ISO8601FormatStyle.DateTimeSeparator, timeSeparator: Date.ISO8601FormatStyle.TimeSeparator) -> Self

Creates a regex component that matches an ISO 8601-formatted date string, capturing the matched substring as a Foundation date in the specified time zone.

static func iso8601WithTimeZone(includingFractionalSeconds: Bool, dateSeparator: Date.ISO8601FormatStyle.DateSeparator, dateTimeSeparator: Date.ISO8601FormatStyle.DateTimeSeparator, timeSeparator: Date.ISO8601FormatStyle.TimeSeparator, timeZoneSeparator: Date.ISO8601FormatStyle.TimeZoneSeparator) -> Self

Creates a regex component that matches an ISO 8601-formatted date string that includes a time zone component, capturing the matched substring as a Foundation date.

### Matching numeric formats

static func localizedInteger(locale: Locale) -> Self

Creates a regex component that matches a localized numeric string, capturing it as an integer value.

static func localizedDouble(locale: Locale) -> Self

Creates a regex component that matches a localized numeric string, capturing it as a double-precision floating-point value.

static func localizedDecimal(locale: Locale) -> Self

Creates a regex component that matches a localized decimal string, capturing it as a Foundation decimal.

static func localizedCurrency(code: Locale.Currency, locale: Locale) -> Self

Creates a regex component that matches a localized currency string, capturing it as a decimal value.

static func localizedIntegerCurrency(code: Locale.Currency, locale: Locale) -> Self

Creates a regex component that matches a localized currency string, capturing it as an integer value.

static func localizedIntegerPercentage(locale: Locale) -> Self

Creates a regex component that matches a localized percentage string, capturing it as a double-precision floating-point value.

static func localizedDoublePercentage(locale: Locale) -> Self

Creates a regex component that matches a localized percentage string, capturing it as a double-precision floating-point value.

### Matching URLs

static func url(scheme: URL.ParseStrategy.ComponentParseStrategy&lt;String>, user: URL.ParseStrategy.ComponentParseStrategy&lt;String>, password: URL.ParseStrategy.ComponentParseStrategy&lt;String>, host: URL.ParseStrategy.ComponentParseStrategy&lt;String>, port: URL.ParseStrategy.ComponentParseStrategy&lt;Int>, path: URL.ParseStrategy.ComponentParseStrategy&lt;String>, query: URL.ParseStrategy.ComponentParseStrategy&lt;String>, fragment: URL.ParseStrategy.ComponentParseStrategy&lt;String>) -> Self

Creates a regex component that matches a URL substring, capturing it as a Foundation URL.

### Supporting types

associatedtype RegexOutput

The output type for this regular expression.

**Required**

typealias DateStyle

A type alias to use when matching date components in a regular expression.

typealias TimeStyle

A type alias to use when matching time components in a regular expression.

## Relationships

### Inherited By

- CustomConsumingRegexComponent

### Conforming Types

- Anchor
- Capture

  Conforms when `Output` conforms to `Copyable` and `Escapable`.

- Character
- CharacterClass
- ChoiceOf

  Conforms when `Output` conforms to `Copyable` and `Escapable`.

- Local

  Conforms when `Output` conforms to `Copyable` and `Escapable`.

- Lookahead

  Conforms when `Output` conforms to `Copyable` and `Escapable`.

- NegativeLookahead

  Conforms when `Output` conforms to `Copyable` and `Escapable`.

- One
- OneOrMore

  Conforms when `Output` conforms to `Copyable` and `Escapable`.

- Optionally

  Conforms when `Output` conforms to `Copyable` and `Escapable`.

- Reference
- Regex
- Repeat

  Conforms when `Output` conforms to `Copyable` and `Escapable`.

- String
- Substring
- TryCapture

  Conforms when `Output` conforms to `Copyable` and `Escapable`.

- Unicode.Scalar
- ZeroOrMore

  Conforms when `Output` conforms to `Copyable` and `Escapable`.

## See Also

### Regular Expressions

struct Regex

A regular expression.

struct RegexRepetitionBehavior

Specifies how much to attempt to match when using a quantifier.

struct RegexSemanticLevel

A semantic level to use during regex matching.

struct RegexWordBoundaryKind

A word boundary algorithm to use during regex matching.

struct AnyRegexOutput

The type-erased, dynamic output of a regular expression match.

protocol CustomConsumingRegexComponent

