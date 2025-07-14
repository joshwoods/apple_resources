

- Swift
- RegexComponent
-  hexDigit 

Type Property

# hexDigit

A character class that matches any hexadecimal digit.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static var hexDigit: CharacterClass { get }
```

Available when `Self` is `CharacterClass`.

## Discussion

`hexDigit` matches the ASCII characters `0` through `9`, and upper- or lowercase `a` through `f`. The corresponding characters in the “Halfwidth and Fullwidth Forms” Unicode block are not matched by this character class.

## See Also

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

static var word: CharacterClass

A character class that matches any element that is a “word character”.

