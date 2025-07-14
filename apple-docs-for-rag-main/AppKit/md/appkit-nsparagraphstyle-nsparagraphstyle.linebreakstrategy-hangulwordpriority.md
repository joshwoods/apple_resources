

- AppKit
- NSParagraphStyle
- NSParagraphStyle.LineBreakStrategy
-  hangulWordPriority 

Type Property

# hangulWordPriority

The text system prohibits breaking between Hangul characters.

macOS 11.0+

``` source
static var hangulWordPriority: NSParagraphStyle.LineBreakStrategy { get }
```

## Discussion

To avoid breaking between Hangul characters, this strategy is preferred for typesetting modern Korean documents that display UI strings.

## See Also

### Getting the line-break styles

static var pushOut: NSParagraphStyle.LineBreakStrategy

The text system pushes out individual lines to avoid an orphan word on the last line of the paragraph.

static var standard: NSParagraphStyle.LineBreakStrategy

The text system uses the same configuration of line-break strategies that it uses for standard UI labels.

