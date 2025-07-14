

- AppKit
- NSTypesetterControlCharacterAction
-  horizontalTabAction 

Type Property

# horizontalTabAction

Treated as tab character.

macOS

``` source
static var horizontalTabAction: NSTypesetterControlCharacterAction { get }
```

## See Also

### Constants

static var zeroAdvancementAction: NSTypesetterControlCharacterAction

Glyphs with this action are filtered out from layout `(notShownAttribute == YES)`.

static var whitespaceAction: NSTypesetterControlCharacterAction

The width for glyphs with this action are determined by boundingBox(forControlGlyphAt:for:proposedLineFragment:glyphPosition:characterIndex:), if the method is implemented; otherwise, same as `NSTypesetterZeroAdvancementAction`.

static var lineBreakAction: NSTypesetterControlCharacterAction

Causes line break.

static var paragraphBreakAction: NSTypesetterControlCharacterAction

Causes paragraph break; the value returned by firstLineHeadIndent is the advancement used for the following glyph.

static var containerBreakAction: NSTypesetterControlCharacterAction

Causes container break.

