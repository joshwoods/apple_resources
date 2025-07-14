

- UIKit
-  NSControlCharacterZeroAdvancementAction Deprecated

Global Variable

# NSControlCharacterZeroAdvancementAction

An action that removes the glyph from layout.

iOS 7.0–9.0DeprecatediPadOS 7.0–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOSDeprecated

``` source
var NSControlCharacterZeroAdvancementAction: Int { get }
```

## Discussion

Glyphs with this action are filtered out from layout (notShownAttribute(forGlyphAt:) `== YES` for the glyph).

## See Also

### Constants

var NSControlCharacterContainerBreakAction: Int

A character that causes a break in layout.

Deprecated

var NSControlCharacterHorizontalTabAction: Int

An action that inserts a horizontal tab.

Deprecated

var NSControlCharacterLineBreakAction: Int

An action that causes a line break.

Deprecated

var NSControlCharacterParagraphBreakAction: Int

An action that causes a paragraph break.

Deprecated

var NSControlCharacterWhitespaceAction: Int

An action that programmatically changes the white space around the glyph.

Deprecated

