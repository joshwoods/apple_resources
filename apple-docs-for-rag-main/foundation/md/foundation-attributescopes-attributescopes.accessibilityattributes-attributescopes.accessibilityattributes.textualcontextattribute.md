

- Foundation
- AttributeScopes
- AttributeScopes.AccessibilityAttributes
-  AttributeScopes.AccessibilityAttributes.TextualContextAttribute 

Enumeration

# AttributeScopes.AccessibilityAttributes.TextualContextAttribute

An attribute for the textual context.

FoundationAccessibilityiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@frozen
enum TextualContextAttribute
```

## Overview

Assistive technologies can use this property to choose an appropriate way to output the text. For example, when encountering a source coding context, VoiceOver could choose to speak all punctuation.

Note

This attribute is not used on macOS

## Topics

### Enumerations

enum TextualContext

Textual context that assistive technologies can use to improve the presentation of spoken text.

## Relationships

### Conforms To

- AttributedStringKey
- BitwiseCopyable
- Copyable
- DecodableAttributedStringKey
- EncodableAttributedStringKey
- MarkdownDecodableAttributedStringKey
- ObjectiveCConvertibleAttributedStringKey
- Sendable

