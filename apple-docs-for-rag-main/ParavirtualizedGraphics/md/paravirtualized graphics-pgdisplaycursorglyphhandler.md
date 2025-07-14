

- Paravirtualized Graphics
-  PGDisplayCursorGlyphHandler 

Type Alias

# PGDisplayCursorGlyphHandler

The block signature for a routine that handles changes to the cursor’s appearance.

Mac Catalyst 14.0+macOS 11.0+

``` source
typealias PGDisplayCursorGlyphHandler = (NSBitmapImageRep, PGDisplayCoord_t) -> Void
```

## Parameters 

`glyph`  

The image to assign to the cursor.

`hotSpot `  

The point to set as the cursor’s hot spot.

## See Also

### Managing Cursor Events

var cursorGlyphHandler: PGDisplayCursorGlyphHandler?

A handler that the framework calls to change the cursor’s appearance.

var cursorShowHandler: PGDisplayCursorShowHandler?

A handler that the framework calls to change the cursor’s visibility.

typealias PGDisplayCursorShowHandler

The block signature for a routine that handles changes to the cursor’s visibility.

