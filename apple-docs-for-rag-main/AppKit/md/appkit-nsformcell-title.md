

- AppKit
- NSFormCell
-  title 

Instance Property

# title

The cell’s title text.

macOS

``` source
@MainActor
var title: String { get set }
```

## Discussion

The default value of this property is `"Field:"`.

## See Also

### Accessing a Cell’s Title

var attributedTitle: NSAttributedString

The title of the cell as an attributed string.

var titleAlignment: NSTextAlignment

The alignment of the title.

var titleBaseWritingDirection: NSWritingDirection

The default writing direction used to render the form cell’s title.

var titleFont: NSFont

The font used to draw cell’s title.

var titleWidth: CGFloat

The width of the title field.

