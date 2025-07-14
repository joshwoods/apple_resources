

- AppKit
- NSLayoutManager
-  typesetterBehavior 

Instance Property

# typesetterBehavior

The default typesetter behavior.

macOS 10.7+

``` source
var typesetterBehavior: NSLayoutManager.TypesetterBehavior { get set }
```

## Discussion

The typesetter behavior affects glyph spacing and line height.

## See Also

### Managing the typesetter

var typesetter: NSTypesetter

The current typesetter.

enum TypesetterBehavior

Constants that determine the layout manager’s behavior during layout.

func defaultLineHeight(for: NSFont) -> CGFloat

Returns the default line height for a line of text that uses a specified font.

func defaultBaselineOffset(for: NSFont) -> CGFloat

Returns the default baseline offset that the layout manager’s typesetter uses for the specified font.

