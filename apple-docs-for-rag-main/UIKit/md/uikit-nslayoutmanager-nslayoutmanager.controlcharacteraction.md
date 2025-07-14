

- UIKit
- NSLayoutManager
-  NSLayoutManager.ControlCharacterAction 

Structure

# NSLayoutManager.ControlCharacterAction

Constants that describe actions for control characters.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
struct ControlCharacterAction
```

## Overview

These constants layoutManager(_:shouldUse:forControlCharacterAt:) delegate method uses.

## Topics

### Actions

static var containerBreak: NSLayoutManager.ControlCharacterAction

An action that triggers a break in layout for the current container.

static var horizontalTab: NSLayoutManager.ControlCharacterAction

An action that inserts a horizontal tab.

static var lineBreak: NSLayoutManager.ControlCharacterAction

An action that causes a line break.

static var paragraphBreak: NSLayoutManager.ControlCharacterAction

An action that causes a paragraph break.

static var whitespace: NSLayoutManager.ControlCharacterAction

An action that adds whitespace.

static var zeroAdvancement: NSLayoutManager.ControlCharacterAction

An action that removes the glyph from layout.

### Initializers

init(rawValue: Int)

Creates a new control character action with the specified raw value.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Invalidating glyphs and layout

func layoutManagerDidInvalidateLayout(NSLayoutManager)

Informs the delegate when the specified layout manager invalidates layout information (not glyph information).

func layoutManager(NSLayoutManager, shouldGenerateGlyphs: UnsafePointer&lt;CGGlyph>, properties: UnsafePointer&lt;NSLayoutManager.GlyphProperty>, characterIndexes: UnsafePointer&lt;Int>, font: UIFont, forGlyphRange: NSRange) -> Int

Enables customization of the initial glyph generation process.

func layoutManager(NSLayoutManager, shouldUse: NSLayoutManager.ControlCharacterAction, forControlCharacterAt: Int) -> NSLayoutManager.ControlCharacterAction

Returns the control character action for the control character at the specified character index.

