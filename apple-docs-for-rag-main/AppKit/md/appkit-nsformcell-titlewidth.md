

- AppKit
- NSFormCell
-  titleWidth 

Instance Property

# titleWidth

The width of the title field.

macOS

``` source
@MainActor
var titleWidth: CGFloat { get set }
```

## Discussion

The width of the title field, measured in points in the user coordinate space. You usually do not need to set this property. AppKit automatically sets the title width whenever the title changes. If the automatic width doesn’t suit your needs, though, you can use this property to set the width explicitly.

After you have set the width this way, AppKit stops setting the width automatically, so you must set this property every time the title changes. If you want AppKit to resume automatic width assignments, set this property to a negative value.

## See Also

### Accessing a Cell’s Title

var attributedTitle: NSAttributedString

The title of the cell as an attributed string.

var title: String

The cell’s title text.

var titleAlignment: NSTextAlignment

The alignment of the title.

var titleBaseWritingDirection: NSWritingDirection

The default writing direction used to render the form cell’s title.

var titleFont: NSFont

The font used to draw cell’s title.

