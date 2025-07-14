

- Foundation
- NSAttributedString
-  NSAttributedString.TextHighlightColorScheme 

Structure

# NSAttributedString.TextHighlightColorScheme

Constants that specify the highlight color to use with the text.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct TextHighlightColorScheme
```

## Overview

Use an NSAttributedString.TextHighlightColorScheme structure as the value of the textHighlightColorScheme attribute. That attribute specifies which color to use when drawing the highlight on the text. This attribute specifies only the color option. To display the highlight itself, add the textHighlightStyle attribute to the text.

## Topics

### Getting the color schemes

static let `default`: NSAttributedString.TextHighlightColorScheme

The default system highlight color.

static let blue: NSAttributedString.TextHighlightColorScheme

A blue highlight color.

static let mint: NSAttributedString.TextHighlightColorScheme

A mint green highlight color.

static let orange: NSAttributedString.TextHighlightColorScheme

An orange highlight color.

static let pink: NSAttributedString.TextHighlightColorScheme

A pink highlight color.

static let purple: NSAttributedString.TextHighlightColorScheme

A purple highlight color.

### Creating a color scheme

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

struct TextHighlightStyle

Constants that specify the type of highlight to apply to text.

struct TextEffectStyle

Constants for the type of effect to apply to the text.

enum SpellingState

Constants for the spelling state attribute key.

struct NSUnderlineStyle

Constants for the underline style and strikethrough style attribute keys.

enum NSWritingDirectionFormatType

Constants for the writing direction attribute key.

