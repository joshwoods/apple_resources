

- AppKit
- NSLayoutManager
- NSLayoutManager.ControlCharacterAction
-  whitespace 

Type Property

# whitespace

An action that adds whitespace.

macOS 10.11+

``` source
static var whitespace: NSLayoutManager.ControlCharacterAction { get }
```

## Discussion

The width for a glyph with this action is determined by the delegate method layoutManager(_:shouldUse:forControlCharacterAt:) if the method is implemented; otherwise, same as `NSControlCharacterZeroAdvancementAction`.

## See Also

### Actions

static var containerBreak: NSLayoutManager.ControlCharacterAction

An action that triggers a break in layout for the current container.

static var horizontalTab: NSLayoutManager.ControlCharacterAction

An action that inserts a horizontal tab.

static var lineBreak: NSLayoutManager.ControlCharacterAction

An action that causes a line break.

static var paragraphBreak: NSLayoutManager.ControlCharacterAction

An action that causes a paragraph break.

static var zeroAdvancement: NSLayoutManager.ControlCharacterAction

An action that removes the glyph from layout.

