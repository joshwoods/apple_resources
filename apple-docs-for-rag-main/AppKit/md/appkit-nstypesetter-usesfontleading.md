

- AppKit
- NSTypesetter
-  usesFontLeading 

Instance Property

# usesFontLeading

Returns whether the typesetter uses the leading (or line gap) value specified in the font metric information of the current font.

macOS

``` source
var usesFontLeading: Bool { get set }
```

## Return Value

true if it uses the information in the font metrics, false otherwise.

## See Also

### Accessing the layout manager

var layoutManager: NSLayoutManager?

Returns the layout manager for the text being typeset.

var typesetterBehavior: NSLayoutManager.TypesetterBehavior

Returns the current typesetter behavior.

var hyphenationFactor: Float

Returns the current hyphenation factor.

