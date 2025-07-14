

- AppKit
- NSATSTypesetter
-  usesFontLeading 

Instance Property

# usesFontLeading

A Boolean value controlling whether the typesetter uses the leading (or line gap) value specified in the font metric information.

macOS

``` source
var usesFontLeading: Bool { get set }
```

## See Also

### Accessing the layout manager

var layoutManager: NSLayoutManager?

The layout manager for the text being typeset.

var typesetterBehavior: NSLayoutManager.TypesetterBehavior

The current typesetter behavior value.

var hyphenationFactor: Float

The threshold controlling when hyphenation is attempted.

var bidiProcessingEnabled: Bool

A Boolean value controlling whether the typesetter performs bidirectional text processing.

