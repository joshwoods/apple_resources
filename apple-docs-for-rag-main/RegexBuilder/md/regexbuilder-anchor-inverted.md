

- RegexBuilder
- Anchor
-  inverted 

Instance Property

# inverted

The inverse of this anchor, which matches at every position that this anchor does not.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
var inverted: Anchor { get }
```

## Discussion

For the wordBoundary and textSegmentBoundary anchors, the inverted version corresponds to `\B` and `\Y`, respectively.

