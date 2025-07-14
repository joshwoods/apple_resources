

- AppKit
- NSLayoutManager
- NSLayoutManager.GlyphProperty
-  controlCharacter 

Type Property

# controlCharacter

A glyph representing a control character.

macOS 10.11+

``` source
static var controlCharacter: NSLayoutManager.GlyphProperty { get }
```

## Discussion

Control character such as tab, attachment, and so on, that has associated special behavior.

## See Also

### Glyph properties

static var null: NSLayoutManager.GlyphProperty

The null glyph, which the layout manager ignores.

static var elastic: NSLayoutManager.GlyphProperty

A glyph with a changeable width, such as a white space character.

static var nonBaseCharacter: NSLayoutManager.GlyphProperty

A glyph that combines several properties.

