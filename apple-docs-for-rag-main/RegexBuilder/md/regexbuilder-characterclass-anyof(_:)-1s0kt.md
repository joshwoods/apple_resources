

- RegexBuilder
- CharacterClass
-  anyOf(\_:) 

Type Method

# anyOf(\_:)

Returns a character class that matches any character in the given string or sequence.

RegexBuilderSwiftiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

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

