

- RegexBuilder
- CharacterClass
-  generalCategory(\_:) 

Type Method

# generalCategory(\_:)

Returns a character class that matches any element with the given Unicode general category.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
static func generalCategory(_ category: Unicode.GeneralCategory) -> CharacterClass
```

## Discussion

For example, when passed `.uppercaseLetter`, this method is equivalent to `/\p{Uppercase_Letter}/` or `/\p{Lu}/`.

