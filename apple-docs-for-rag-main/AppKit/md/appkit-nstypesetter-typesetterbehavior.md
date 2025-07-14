

- AppKit
- NSTypesetter
-  typesetterBehavior 

Instance Property

# typesetterBehavior

Returns the current typesetter behavior.

macOS

``` source
var typesetterBehavior: NSLayoutManager.TypesetterBehavior { get set }
```

## Return Value

The current typesetter behavior.

## See Also

### Accessing the layout manager

var layoutManager: NSLayoutManager?

Returns the layout manager for the text being typeset.

var usesFontLeading: Bool

Returns whether the typesetter uses the leading (or line gap) value specified in the font metric information of the current font.

var hyphenationFactor: Float

Returns the current hyphenation factor.

