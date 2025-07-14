

- RegexBuilder
- Anchor
-  wordBoundary 

Type Property

# wordBoundary

An anchor that matches at a word boundary.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
static var wordBoundary: Anchor { get }
```

## Discussion

Word boundaries are identified using the Unicode default word boundary algorithm by default. To specify a different word boundary algorithm, use the `wordBoundaryKind(_:)` method.

This anchor is equivalent to `\b` in regex syntax.

