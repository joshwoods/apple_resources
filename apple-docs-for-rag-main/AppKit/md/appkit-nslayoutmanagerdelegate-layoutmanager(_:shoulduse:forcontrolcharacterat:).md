

- AppKit
- NSLayoutManagerDelegate
-  layoutManager(\_:shouldUse:forControlCharacterAt:) 

Instance Method

# layoutManager(\_:shouldUse:forControlCharacterAt:)

Returns the control character action for the control character at the specified character index.

macOS 10.11+

``` source
optional func layoutManager(
    _ layoutManager: NSLayoutManager,
    shouldUse action: NSLayoutManager.ControlCharacterAction,
    forControlCharacterAt charIndex: Int
) -> NSLayoutManager.ControlCharacterAction
```

## Parameters 

`layoutManager`  

The layout manager doing the layout.

`action`  

The proposed control character action for the character at the given index. Possible values are enumerated by NSLayoutManager.ControlCharacterAction.

`charIndex`  

The index of the control character for which the action is proposed.

## Return Value

The control character action for the control character at the given index.

## See Also

### Invalidating glyphs and layout

func layoutManagerDidInvalidateLayout(NSLayoutManager)

Informs the delegate when the specified layout manager invalidates layout information (not glyph information).

func layoutManager(NSLayoutManager, shouldGenerateGlyphs: UnsafePointer&lt;CGGlyph>, properties: UnsafePointer&lt;NSLayoutManager.GlyphProperty>, characterIndexes: UnsafePointer&lt;Int>, font: NSFont, forGlyphRange: NSRange) -> Int

Enables customization of the initial glyph generation process.

struct ControlCharacterAction

Constants that describe actions for control characters.

