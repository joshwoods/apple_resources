

- Paravirtualized Graphics
-  PGDisplayCursorShowHandler 

Type Alias

# PGDisplayCursorShowHandler

The block signature for a routine that handles changes to the cursor’s visibility.

Mac Catalyst 14.0+macOS 11.0+

``` source
typealias PGDisplayCursorShowHandler = (Bool) -> Void
```

## Parameters 

`show`  

A Boolean value that indicates whether to show the cursor.

## See Also

### Managing Cursor Events

var cursorGlyphHandler: PGDisplayCursorGlyphHandler?

A handler that the framework calls to change the cursor’s appearance.

var cursorShowHandler: PGDisplayCursorShowHandler?

A handler that the framework calls to change the cursor’s visibility.

typealias PGDisplayCursorGlyphHandler

The block signature for a routine that handles changes to the cursor’s appearance.

