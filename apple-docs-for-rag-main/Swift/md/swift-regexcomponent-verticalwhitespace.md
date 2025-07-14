

- Swift
- RegexComponent
-  verticalWhitespace 

Type Property

# verticalWhitespace

A character class that matches any element that is classified as vertical whitespace.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static var verticalWhitespace: CharacterClass { get }
```

Available when `Self` is `CharacterClass`.

## Discussion

This character class is equivalent to `\v` in regex syntax.

## See Also

### Matching whitespace and line endings

static var horizontalWhitespace: CharacterClass

A character class that matches any element that is classified as horizontal whitespace.

static var newlineSequence: CharacterClass

A character class that matches any newline sequence.

static var whitespace: CharacterClass

A character class that matches any element that is classified as whitespace.

