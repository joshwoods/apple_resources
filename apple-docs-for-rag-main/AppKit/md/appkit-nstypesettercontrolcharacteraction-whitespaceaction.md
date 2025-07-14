

- AppKit
- NSTypesetterControlCharacterAction
-  whitespaceAction 

Type Property

# whitespaceAction

The width for glyphs with this action are determined by boundingBox(forControlGlyphAt:for:proposedLineFragment:glyphPosition:characterIndex:), if the method is implemented; otherwise, same as `NSTypesetterZeroAdvancementAction`.

macOS

``` source
static var whitespaceAction: NSTypesetterControlCharacterAction { get }
```

## See Also

### Constants

static var zeroAdvancementAction: NSTypesetterControlCharacterAction

Glyphs with this action are filtered out from layout `(notShownAttribute == YES)`.

static var horizontalTabAction: NSTypesetterControlCharacterAction

Treated as tab character.

static var lineBreakAction: NSTypesetterControlCharacterAction

Causes line break.

static var paragraphBreakAction: NSTypesetterControlCharacterAction

Causes paragraph break; the value returned by firstLineHeadIndent is the advancement used for the following glyph.

static var containerBreakAction: NSTypesetterControlCharacterAction

Causes container break.

