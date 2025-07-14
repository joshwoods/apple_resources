

- AppKit
- NSATSTypesetter
-  typesetterBehavior 

Instance Property

# typesetterBehavior

The current typesetter behavior value.

macOS

``` source
var typesetterBehavior: NSLayoutManager.TypesetterBehavior { get set }
```

## See Also

### Accessing the layout manager

var layoutManager: NSLayoutManager?

The layout manager for the text being typeset.

var usesFontLeading: Bool

A Boolean value controlling whether the typesetter uses the leading (or line gap) value specified in the font metric information.

var hyphenationFactor: Float

The threshold controlling when hyphenation is attempted.

var bidiProcessingEnabled: Bool

A Boolean value controlling whether the typesetter performs bidirectional text processing.

