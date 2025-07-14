

- Paravirtualized Graphics
- PGDisplayDescriptor
-  cursorGlyphHandler 

Instance Property

# cursorGlyphHandler

A handler that the framework calls to change the cursor’s appearance.

Mac Catalyst 14.0+macOS 11.0+

``` source
var cursorGlyphHandler: PGDisplayCursorGlyphHandler? { get set }
```

## See Also

### Managing Cursor Events

var cursorShowHandler: PGDisplayCursorShowHandler?

A handler that the framework calls to change the cursor’s visibility.

typealias PGDisplayCursorGlyphHandler

The block signature for a routine that handles changes to the cursor’s appearance.

typealias PGDisplayCursorShowHandler

The block signature for a routine that handles changes to the cursor’s visibility.

