

- RegexBuilder
- CharacterClass
-  hexDigit 

Type Property

# hexDigit

A character class that matches any hexadecimal digit.

RegexBuilderSwiftiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
static var hexDigit: CharacterClass { get }
```

Available when `Self` is `CharacterClass`.

## Discussion

`hexDigit` matches the ASCII characters `0` through `9`, and upper- or lowercase `a` through `f`. The corresponding characters in the “Halfwidth and Fullwidth Forms” Unicode block are not matched by this character class.

