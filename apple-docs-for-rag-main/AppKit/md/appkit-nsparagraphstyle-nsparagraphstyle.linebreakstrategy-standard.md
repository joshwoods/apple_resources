

- AppKit
- NSParagraphStyle
- NSParagraphStyle.LineBreakStrategy
-  standard 

Type Property

# standard

The text system uses the same configuration of line-break strategies that it uses for standard UI labels.

macOS 11.0+

``` source
static var standard: NSParagraphStyle.LineBreakStrategy { get }
```

## Discussion

This strategy optimizes for displaying shorter strings that are common in UI labels. This strategy may be unsuitable for large amounts of text.

## See Also

### Getting the line-break styles

static var pushOut: NSParagraphStyle.LineBreakStrategy

The text system pushes out individual lines to avoid an orphan word on the last line of the paragraph.

static var hangulWordPriority: NSParagraphStyle.LineBreakStrategy

The text system prohibits breaking between Hangul characters.

