

- RegexBuilder
- CharacterClass
-  anyGraphemeCluster 

Type Property

# anyGraphemeCluster

A character class that matches any single `Character`, or extended grapheme cluster, regardless of the current semantic level.

RegexBuilderSwiftiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
static var anyGraphemeCluster: CharacterClass { get }
```

Available when `Self` is `CharacterClass`.

## Discussion

This character class is equivalent to `\X` in regex syntax.

