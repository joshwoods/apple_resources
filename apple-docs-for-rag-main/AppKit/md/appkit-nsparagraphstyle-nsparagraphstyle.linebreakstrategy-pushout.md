

- AppKit
- NSParagraphStyle
- NSParagraphStyle.LineBreakStrategy
-  pushOut 

Type Property

# pushOut

The text system pushes out individual lines to avoid an orphan word on the last line of the paragraph.

macOS 10.11+

``` source
static var pushOut: NSParagraphStyle.LineBreakStrategy { get }
```

## Discussion

To avoid an orphan word on the last line of a paragraph before a page break, the text system may extend individual lines by one or more words. Typically, the text system only pushes out the last line by one word.

## See Also

### Getting the line-break styles

static var hangulWordPriority: NSParagraphStyle.LineBreakStrategy

The text system prohibits breaking between Hangul characters.

static var standard: NSParagraphStyle.LineBreakStrategy

The text system uses the same configuration of line-break strategies that it uses for standard UI labels.

