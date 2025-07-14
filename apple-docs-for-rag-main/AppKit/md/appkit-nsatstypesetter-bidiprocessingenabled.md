

- AppKit
- NSATSTypesetter
-  bidiProcessingEnabled 

Instance Property

# bidiProcessingEnabled

A Boolean value controlling whether the typesetter performs bidirectional text processing.

macOS

``` source
var bidiProcessingEnabled: Bool { get set }
```

## Discussion

You can use this method to disable the bidirectional layout stage if you know the paragraph does not need this stage; that is, if the characters in the backing store are in display order.

## See Also

### Accessing the layout manager

var layoutManager: NSLayoutManager?

The layout manager for the text being typeset.

var usesFontLeading: Bool

A Boolean value controlling whether the typesetter uses the leading (or line gap) value specified in the font metric information.

var typesetterBehavior: NSLayoutManager.TypesetterBehavior

The current typesetter behavior value.

var hyphenationFactor: Float

The threshold controlling when hyphenation is attempted.

