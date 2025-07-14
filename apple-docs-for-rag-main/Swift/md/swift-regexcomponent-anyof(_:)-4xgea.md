

- Swift
- RegexComponent
-  anyOf(\_:) 

Type Method

# anyOf(\_:)

Returns a character class that matches any character in the given string or sequence.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func anyOf(_ s: S) -> CharacterClass where S : Sequence, S.Element == Character
```

Available when `Self` is `CharacterClass`.

## Discussion

Calling this method with a group of characters is equivalent to listing those characters in a custom character class in regex syntax. For example, the two regexes in this example are equivalent:

```
let regex1 = /[abcd]+/
let regex2 = OneOrMore(.anyOf("abcd"))
```

## See Also

### Matching substring sequences

static func anyOf&lt;S>(S) -> CharacterClass

Returns a character class that matches any Unicode scalar in the given sequence.

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

