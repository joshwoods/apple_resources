

- Core Animation
- CATextLayerTruncationMode
-  none 

Type Property

# none

Each line is displayed so that the text is either wrapped or clipped.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
static let none: CATextLayerTruncationMode
```

## Discussion

If the isWrapped property is true, the text is wrapped to the receiver’s bounds, otherwise the text is clipped to the receiver’s bounds.

## See Also

### Constants

static let start: CATextLayerTruncationMode

Each line is displayed so that the end fits in the container and the missing text is indicated by some kind of ellipsis glyph.

static let end: CATextLayerTruncationMode

Each line is displayed so that the beginning fits in the container and the missing text is indicated by some kind of ellipsis glyph.

static let middle: CATextLayerTruncationMode

Each line is displayed so that the beginning and end fit in the container and the missing text is indicated by some kind of ellipsis glyph in the middle.

