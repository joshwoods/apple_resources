

- AppKit
- NSTypesetterControlCharacterAction
-  zeroAdvancementAction 

Type Property

# zeroAdvancementAction

Glyphs with this action are filtered out from layout `(notShownAttribute == YES)`.

macOS

``` source
static var zeroAdvancementAction: NSTypesetterControlCharacterAction { get }
```

## See Also

### Constants

static var whitespaceAction: NSTypesetterControlCharacterAction

The width for glyphs with this action are determined by boundingBox(forControlGlyphAt:for:proposedLineFragment:glyphPosition:characterIndex:), if the method is implemented; otherwise, same as `NSTypesetterZeroAdvancementAction`.

static var horizontalTabAction: NSTypesetterControlCharacterAction

Treated as tab character.

static var lineBreakAction: NSTypesetterControlCharacterAction

Causes line break.

static var paragraphBreakAction: NSTypesetterControlCharacterAction

Causes paragraph break; the value returned by firstLineHeadIndent is the advancement used for the following glyph.

static var containerBreakAction: NSTypesetterControlCharacterAction

Causes container break.

