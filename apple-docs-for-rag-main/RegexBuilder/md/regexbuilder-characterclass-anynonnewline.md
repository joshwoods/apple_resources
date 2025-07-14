

- RegexBuilder
- CharacterClass
-  anyNonNewline 

Type Property

# anyNonNewline

A character class that matches any element that isn’t a newline.

RegexBuilderSwiftiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
static var anyNonNewline: CharacterClass { get }
```

Available when `Self` is `CharacterClass`.

## Discussion

This character class is unaffected by the `dotMatchesNewlines()` method. To match any character, including newlines, see any.

This character class is equivalent to the regex syntax “dot” metacharacter with single-line mode disabled: `(?-s:.)`.

