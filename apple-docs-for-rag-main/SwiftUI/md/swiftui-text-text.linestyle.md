

- SwiftUI
- Text
-  Text.LineStyle 

Structure

# Text.LineStyle

Description of the style used to draw the line for `StrikethroughStyleAttribute` and `UnderlineStyleAttribute`.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct LineStyle
```

## Overview

Use this type to specify `underlineStyle` and `strikethroughStyle` SwiftUI attributes of an `AttributedString`.

## Topics

### Getting text line styles

static let single: Text.LineStyle

Draw a single solid line.

### Creating a text line style

init?(nsUnderlineStyle: NSUnderlineStyle)

Creates a `Text.LineStyle` from `NSUnderlineStyle`.

init(pattern: Text.LineStyle.Pattern, color: Color?)

Creates a line style.

struct Pattern

The pattern, that the line has.

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Styling the view’s text

func foregroundStyle&lt;S>(S) -> Text

Sets the style of the text displayed by this view.

func bold() -> Text

Applies a bold font weight to the text.

func bold(Bool) -> Text

Applies a bold font weight to the text.

func italic() -> Text

Applies italics to the text.

func italic(Bool) -> Text

Applies italics to the text.

func strikethrough(Bool, color: Color?) -> Text

Applies a strikethrough to the text.

func strikethrough(Bool, pattern: Text.LineStyle.Pattern, color: Color?) -> Text

Applies a strikethrough to the text.

func underline(Bool, color: Color?) -> Text

Applies an underline to the text.

func underline(Bool, pattern: Text.LineStyle.Pattern, color: Color?) -> Text

Applies an underline to the text.

func monospaced(Bool) -> Text

Modifies the font of the text to use the fixed-width variant of the current font, if possible.

func monospacedDigit() -> Text

Modifies the text view’s font to use fixed-width digits, while leaving other characters proportionally spaced.

func kerning(CGFloat) -> Text

Sets the spacing, or kerning, between characters.

func tracking(CGFloat) -> Text

Sets the tracking for the text.

func baselineOffset(CGFloat) -> Text

Sets the vertical offset for the text relative to its baseline.

enum Case

A scheme for transforming the capitalization of characters within text.

