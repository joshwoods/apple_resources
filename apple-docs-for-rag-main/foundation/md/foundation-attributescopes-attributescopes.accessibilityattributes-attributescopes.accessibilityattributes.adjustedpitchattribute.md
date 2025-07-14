

- Foundation
- AttributeScopes
- AttributeScopes.AccessibilityAttributes
-  AttributeScopes.AccessibilityAttributes.AdjustedPitchAttribute 

Enumeration

# AttributeScopes.AccessibilityAttributes.AdjustedPitchAttribute

An attribute to adjust the pitch the spoken speech.

FoundationAccessibilityiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@frozen
enum AdjustedPitchAttribute
```

## Overview

Values between `-1` and `0` result in a lower pitch while values between `0` and `1` result in a higher pitch.

For example, you may want to lower the pitch when an object is deleted, or raise the pitch if an object is inserted.

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

