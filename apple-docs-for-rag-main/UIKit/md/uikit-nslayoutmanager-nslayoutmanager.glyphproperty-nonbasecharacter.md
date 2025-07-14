

- UIKit
- NSLayoutManager
- NSLayoutManager.GlyphProperty
-  nonBaseCharacter 

Type Property

# nonBaseCharacter

A glyph that combines several properties.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
static var nonBaseCharacter: NSLayoutManager.GlyphProperty { get }
```

## Discussion

A glyph of this type typically represents characters in the Unicode Mn class.

## See Also

### Glyph properties

static var null: NSLayoutManager.GlyphProperty

The null glyph, which the layout manager ignores.

static var controlCharacter: NSLayoutManager.GlyphProperty

A glyph representing a control character.

static var elastic: NSLayoutManager.GlyphProperty

A glyph with a changeable width, such as a white space character.

