

- RegexBuilder
- CharacterClass
-  anyOf(\_:) 

Type Method

# anyOf(\_:)

Returns a character class that matches any Unicode scalar in the given sequence.

RegexBuilderSwiftiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
static func anyOf(_ s: S) -> CharacterClass where S : Sequence, S.Element == Unicode.Scalar
```

Available when `Self` is `CharacterClass`.

## Discussion

Calling this method with a group of Unicode scalars is equivalent to listing them in a custom character class in regex syntax.

