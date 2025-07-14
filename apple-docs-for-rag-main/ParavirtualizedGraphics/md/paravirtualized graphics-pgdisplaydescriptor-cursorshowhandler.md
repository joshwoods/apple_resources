

- Paravirtualized Graphics
- PGDisplayDescriptor
-  cursorShowHandler 

Instance Property

# cursorShowHandler

A handler that the framework calls to change the cursor’s visibility.

Mac Catalyst 14.0+macOS 11.0+

``` source
var cursorShowHandler: PGDisplayCursorShowHandler? { get set }
```

## See Also

### Managing Cursor Events

var cursorGlyphHandler: PGDisplayCursorGlyphHandler?

A handler that the framework calls to change the cursor’s appearance.

typealias PGDisplayCursorGlyphHandler

The block signature for a routine that handles changes to the cursor’s appearance.

typealias PGDisplayCursorShowHandler

The block signature for a routine that handles changes to the cursor’s visibility.

