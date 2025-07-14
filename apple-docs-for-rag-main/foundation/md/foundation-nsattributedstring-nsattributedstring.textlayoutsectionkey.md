

- Foundation
- NSAttributedString
-  NSAttributedString.TextLayoutSectionKey 

Structure

# NSAttributedString.TextLayoutSectionKey

Constants for the text layout sections document attribute key.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct TextLayoutSectionKey
```

## Overview

Use these constants as values for the textLayoutSections key in the document attributes dictionary.

## Topics

### Getting keys for text layouts

static let orientation: NSAttributedString.TextLayoutSectionKey

The orientation of the text.

static let range: NSAttributedString.TextLayoutSectionKey

The character range.

### Initializers

init(rawValue: String)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting document-wide attributes

struct DocumentAttributeKey

The attributes you apply to an entire document.

struct DocumentReadingOptionKey

Options for constructing an attributed string from data you read from disk.

HTML attributes

Documentwide attributes that provide control over the form of generated HTML.

struct DocumentType

Constants for the document type document attribute key.

enum NSTextScalingType

Constants that specify the text scaling.

