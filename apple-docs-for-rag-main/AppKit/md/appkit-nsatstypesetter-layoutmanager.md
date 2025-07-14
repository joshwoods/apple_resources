

- AppKit
- NSATSTypesetter
-  layoutManager 

Instance Property

# layoutManager

The layout manager for the text being typeset.

macOS

``` source
unowned(unsafe) var layoutManager: NSLayoutManager? { get }
```

## See Also

### Accessing the layout manager

var usesFontLeading: Bool

A Boolean value controlling whether the typesetter uses the leading (or line gap) value specified in the font metric information.

var typesetterBehavior: NSLayoutManager.TypesetterBehavior

The current typesetter behavior value.

var hyphenationFactor: Float

The threshold controlling when hyphenation is attempted.

var bidiProcessingEnabled: Bool

A Boolean value controlling whether the typesetter performs bidirectional text processing.

