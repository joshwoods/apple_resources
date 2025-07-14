

- Foundation
- NSAttributedString
- NSAttributedString.Key
-  writingDirection 

Type Property

# writingDirection

The writing direction of the text.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let writingDirection: NSAttributedString.Key
```

## Discussion

The value of this attribute is an NSArray object containing NSNumber objects representing the nested levels of writing direction overrides, in order from outermost to innermost.

This attribute provides a means to override the default bidirectional text algorithm, equivalent to using the Unicode bidi control characters `LRE`, `RLE`, `LRO`, or `RLO` paired with `PDF`, but as a higher-level attribute. (See Unicode Standard Annex #9 for information about the Unicode bidi formatting codes.) The `NSWritingDirectionAttributeName` constant is a character-level attribute that provides a higher-level alternative to the inclusion of explicit bidirectional control characters in text. It is the `NSAttributedString` equivalent of the HTML markup using `bdo` element with the `dir` attribute.

The values of the `NSNumber` objects should be `0`, `1`, `2`, or `3`, for `LRE`, `RLE`, `LRO`, or `RLO` respectively, and combinations of NSWritingDirection.leftToRight and NSWritingDirection.rightToLeft with NSTextWritingDirectionEmbedding or `NSTextWritingDirectionOverride`, as shown in doc:#Table-1.

| Array NSNumber Values | Unicode Control Characters | Writing Direction Constants |
|----|----|----|
| `0` | `LRE` | `NSWritingDirectionLeftToRight` \| `NSTextWritingDirectionEmbedding` |
| `1` | `RLE` | `NSWritingDirectionRightToLeft` \| `NSTextWritingDirectionEmbedding` |
| `2` | `LRO` | `NSWritingDirectionLeftToRight` \| `NSTextWritingDirectionOverride` |
| `3` | `RLO` | `NSWritingDirectionRightToLeft` \| `NSTextWritingDirectionOverride` |

## See Also

### Getting rendering attribute keys

static let backgroundColor: NSAttributedString.Key

The color of the background behind the text.

static let baselineOffset: NSAttributedString.Key

The vertical offset for the position of the text.

static let font: NSAttributedString.Key

The font of the text.

static let foregroundColor: NSAttributedString.Key

The color of the text.

static let glyphInfo: NSAttributedString.Key

The name of a glyph info object.

static let kern: NSAttributedString.Key

The kerning of the text.

static let ligature: NSAttributedString.Key

The ligature of the text.

static let paragraphStyle: NSAttributedString.Key

The paragraph style of the text.

static let strikethroughColor: NSAttributedString.Key

The color of the strikethrough.

static let strikethroughStyle: NSAttributedString.Key

The strikethrough style of the text.

static let strokeColor: NSAttributedString.Key

The color of the stroke.

static let strokeWidth: NSAttributedString.Key

The width of the stroke.

static let superscript: NSAttributedString.Key

The superscript of the text.

static let tracking: NSAttributedString.Key

The amount to modify the default tracking.

static let underlineColor: NSAttributedString.Key

The color of the underline.

