

- AppKit
- NSTypesetter
-  layoutManager 

Instance Property

# layoutManager

Returns the layout manager for the text being typeset.

macOS

``` source
unowned(unsafe) var layoutManager: NSLayoutManager? { get }
```

## Return Value

The layout manager for the text being typeset. This value is valid only while the typesetter is performing layout.

## See Also

### Accessing the layout manager

var usesFontLeading: Bool

Returns whether the typesetter uses the leading (or line gap) value specified in the font metric information of the current font.

var typesetterBehavior: NSLayoutManager.TypesetterBehavior

Returns the current typesetter behavior.

var hyphenationFactor: Float

Returns the current hyphenation factor.

