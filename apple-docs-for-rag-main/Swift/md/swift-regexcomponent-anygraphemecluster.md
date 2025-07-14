

- Swift
- RegexComponent
-  anyGraphemeCluster 

Type Property

# anyGraphemeCluster

A character class that matches any single `Character`, or extended grapheme cluster, regardless of the current semantic level.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static var anyGraphemeCluster: CharacterClass { get }
```

Available when `Self` is `CharacterClass`.

## Discussion

This character class is equivalent to `\X` in regex syntax.

## See Also

### Matching substring sequences

static func anyOf&lt;S>(S) -> CharacterClass

Returns a character class that matches any Unicode scalar in the given sequence.

static func anyOf&lt;S>(S) -> CharacterClass

Returns a character class that matches any character in the given string or sequence.

static var any: CharacterClass

A character class that matches any element.

static var anyNonNewline: CharacterClass

A character class that matches any element that isn’t a newline.

static var digit: CharacterClass

A character class that matches any digit.

static var hexDigit: CharacterClass

A character class that matches any hexadecimal digit.

static var word: CharacterClass

A character class that matches any element that is a “word character”.

