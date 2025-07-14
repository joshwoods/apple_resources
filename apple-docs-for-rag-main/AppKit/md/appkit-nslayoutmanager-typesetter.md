

- AppKit
- NSLayoutManager
-  typesetter 

Instance Property

# typesetter

The current typesetter.

macOS 10.7+

``` source
var typesetter: NSTypesetter { get set }
```

## See Also

### Managing the typesetter

var typesetterBehavior: NSLayoutManager.TypesetterBehavior

The default typesetter behavior.

enum TypesetterBehavior

Constants that determine the layout manager’s behavior during layout.

func defaultLineHeight(for: NSFont) -> CGFloat

Returns the default line height for a line of text that uses a specified font.

func defaultBaselineOffset(for: NSFont) -> CGFloat

Returns the default baseline offset that the layout manager’s typesetter uses for the specified font.

