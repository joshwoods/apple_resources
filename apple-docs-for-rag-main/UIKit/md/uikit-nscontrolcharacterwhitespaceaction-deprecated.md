

- UIKit
-  NSControlCharacterWhitespaceAction Deprecated

Global Variable

# NSControlCharacterWhitespaceAction

An action that programmatically changes the white space around the glyph.

iOS 7.0–9.0DeprecatediPadOS 7.0–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOSDeprecated

``` source
var NSControlCharacterWhitespaceAction: Int { get }
```

## Discussion

The width for a glyph with this action is determined by the delegate method layoutManager(_:boundingBoxForControlGlyphAt:for:proposedLineFragment:glyphPosition:characterIndex:) if the method is implemented; otherwise, same as `NSControlCharacterZeroAdvancementAction`.

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

var NSControlCharacterZeroAdvancementAction: Int

An action that removes the glyph from layout.

Deprecated

