

- AppKit
- NSLayoutManagerDelegate
-  layoutManagerDidInvalidateLayout(\_:) 

Instance Method

# layoutManagerDidInvalidateLayout(\_:)

Informs the delegate when the specified layout manager invalidates layout information (not glyph information).

macOS 10.0+

``` source
optional func layoutManagerDidInvalidateLayout(_ sender: NSLayoutManager)
```

## Parameters 

`sender`  

The layout manager that invalidated layout.

## Discussion

This method is invoked only when layout was complete and then became invalidated for some reason. Delegates can use this information to show an indicator of background layout or to enable a button that forces immediate layout of text.

## See Also

### Invalidating glyphs and layout

func layoutManager(NSLayoutManager, shouldGenerateGlyphs: UnsafePointer&lt;CGGlyph>, properties: UnsafePointer&lt;NSLayoutManager.GlyphProperty>, characterIndexes: UnsafePointer&lt;Int>, font: NSFont, forGlyphRange: NSRange) -> Int

Enables customization of the initial glyph generation process.

func layoutManager(NSLayoutManager, shouldUse: NSLayoutManager.ControlCharacterAction, forControlCharacterAt: Int) -> NSLayoutManager.ControlCharacterAction

Returns the control character action for the control character at the specified character index.

struct ControlCharacterAction

Constants that describe actions for control characters.

