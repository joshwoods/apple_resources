

- AppKit
- NSLayoutManager
- NSLayoutManager.ControlCharacterAction
-  paragraphBreak 

Type Property

# paragraphBreak

An action that causes a paragraph break.

macOS 10.11+

``` source
static var paragraphBreak: NSLayoutManager.ControlCharacterAction { get }
```

## Discussion

The value in firstLineHeadIndent is used for the following glyph.

## See Also

### Actions

static var containerBreak: NSLayoutManager.ControlCharacterAction

An action that triggers a break in layout for the current container.

static var horizontalTab: NSLayoutManager.ControlCharacterAction

An action that inserts a horizontal tab.

static var lineBreak: NSLayoutManager.ControlCharacterAction

An action that causes a line break.

static var whitespace: NSLayoutManager.ControlCharacterAction

An action that adds whitespace.

static var zeroAdvancement: NSLayoutManager.ControlCharacterAction

An action that removes the glyph from layout.

