

- RegexBuilder
- CharacterClass
-  any 

Type Property

# any

A character class that matches any element.

RegexBuilderSwiftiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
static var any: CharacterClass { get }
```

Available when `Self` is `CharacterClass`.

## Discussion

This character class is unaffected by the `dotMatchesNewlines()` method. To match any character that isn’t a newline, see anyNonNewline.

This character class is equivalent to the regex syntax “dot” metacharacter in single-line mode: `(?s:.)`.

