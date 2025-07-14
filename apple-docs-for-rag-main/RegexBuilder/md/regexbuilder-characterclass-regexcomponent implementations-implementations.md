

- RegexBuilder
- CharacterClass
-  RegexComponent Implementations 

API Collection

# RegexComponent Implementations

## Topics

### Initializers

init(CharacterClass, CharacterClass...)

Creates a character class that combines the given classes in a union.

### Instance Properties

var regex: Regex&lt;Substring>

The regular expression represented by this component.

### Type Aliases

typealias RegexOutput

The output type for this regular expression.

### Type Properties

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

static var horizontalWhitespace: CharacterClass

A character class that matches any element that is classified as horizontal whitespace.

static var newlineSequence: CharacterClass

A character class that matches any newline sequence.

static var verticalWhitespace: CharacterClass

A character class that matches any element that is classified as vertical whitespace.

static var whitespace: CharacterClass

A character class that matches any element that is classified as whitespace.

static var word: CharacterClass

A character class that matches any element that is a “word character”.

### Type Methods

static func anyOf&lt;S>(S) -> CharacterClass

Returns a character class that matches any character in the given string or sequence.

static func anyOf&lt;S>(S) -> CharacterClass

Returns a character class that matches any Unicode scalar in the given sequence.

