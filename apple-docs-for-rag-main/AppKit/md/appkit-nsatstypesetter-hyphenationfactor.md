

- AppKit
- NSATSTypesetter
-  hyphenationFactor 

Instance Property

# hyphenationFactor

The threshold controlling when hyphenation is attempted.

macOS

``` source
var hyphenationFactor: Float { get set }
```

## See Also

### Accessing the layout manager

var layoutManager: NSLayoutManager?

The layout manager for the text being typeset.

var usesFontLeading: Bool

A Boolean value controlling whether the typesetter uses the leading (or line gap) value specified in the font metric information.

var typesetterBehavior: NSLayoutManager.TypesetterBehavior

The current typesetter behavior value.

var bidiProcessingEnabled: Bool

A Boolean value controlling whether the typesetter performs bidirectional text processing.

