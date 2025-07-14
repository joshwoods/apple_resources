

- AppKit
- NSFormCell
-  titleAlignment 

Instance Property

# titleAlignment

The alignment of the title.

macOS

``` source
@MainActor
var titleAlignment: NSTextAlignment { get set }
```

## Discussion

The alignment can be one of the following values: `NSLeftTextAlignment`, `NSCenterTextAlignment`, or `NSRightTextAlignment`. The default alignment is `NSRightTextAlignment`.

## See Also

### Accessing a Cell’s Title

var attributedTitle: NSAttributedString

The title of the cell as an attributed string.

var title: String

The cell’s title text.

var titleBaseWritingDirection: NSWritingDirection

The default writing direction used to render the form cell’s title.

var titleFont: NSFont

The font used to draw cell’s title.

var titleWidth: CGFloat

The width of the title field.

