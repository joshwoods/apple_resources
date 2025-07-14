

- Foundation
- NSAttributedString
-  NSAttributedString.TextHighlightStyle 

Structure

# NSAttributedString.TextHighlightStyle

Constants that specify the type of highlight to apply to text.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct TextHighlightStyle
```

## Overview

Use an NSAttributedString.TextHighlightStyle structure as the value of the textHighlightStyle attribute. That attribute applies a highlight to the text to emphasize it. The highlight contributes a background color and a contrasting foreground color to the text.

## Topics

### Getting the highlight styles

static let `default`: NSAttributedString.TextHighlightStyle

The default highlight style to apply to text.

### Creating a highlight style

init(String)

init(rawValue: String)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting text content attributes

struct Key

The attributes you apply to ranges of characters in an attributed string.

struct TextHighlightColorScheme

Constants that specify the highlight color to use with the text.

struct TextEffectStyle

Constants for the type of effect to apply to the text.

enum SpellingState

Constants for the spelling state attribute key.

struct NSUnderlineStyle

Constants for the underline style and strikethrough style attribute keys.

enum NSWritingDirectionFormatType

Constants for the writing direction attribute key.

