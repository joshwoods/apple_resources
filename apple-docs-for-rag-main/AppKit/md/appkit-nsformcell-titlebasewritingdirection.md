

- AppKit
- NSFormCell
-  titleBaseWritingDirection 

Instance Property

# titleBaseWritingDirection

The default writing direction used to render the form cell’s title.

macOS

``` source
@MainActor
var titleBaseWritingDirection: NSWritingDirection { get set }
```

## Discussion

Can be one of the following constants: `NSWritingDirectionNatural`, `NSWritingDirectionLeftToRight`, or `NSWritingDirectionRightToLeft`.

## See Also

### Accessing a Cell’s Title

var attributedTitle: NSAttributedString

The title of the cell as an attributed string.

var title: String

The cell’s title text.

var titleAlignment: NSTextAlignment

The alignment of the title.

var titleFont: NSFont

The font used to draw cell’s title.

var titleWidth: CGFloat

The width of the title field.

