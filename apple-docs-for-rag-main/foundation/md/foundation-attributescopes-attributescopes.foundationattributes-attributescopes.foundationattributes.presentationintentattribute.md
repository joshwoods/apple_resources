

- Foundation
- AttributeScopes
- AttributeScopes.FoundationAttributes
-  AttributeScopes.FoundationAttributes.PresentationIntentAttribute 

Enumeration

# AttributeScopes.FoundationAttributes.PresentationIntentAttribute

A type for using a presentation intent as an attribute.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@frozen
enum PresentationIntentAttribute
```

## Overview

A presentation intent applies a block of characters, and covers traits like list, block quote, or table presentation.

## Relationships

### Conforms To

- AttributedStringKey
- BitwiseCopyable
- Copyable
- DecodableAttributedStringKey
- EncodableAttributedStringKey

## See Also

### Using presentation intent attributes

let inlinePresentationIntent: AttributeScopes.FoundationAttributes.InlinePresentationIntentAttribute

A property for accessing an inline presentation intent attribute.

enum InlinePresentationIntentAttribute

A type for using an inline presentation intent as an attribute.

struct InlinePresentationIntent

A type that defines presentation intent for runs of characters for traits like emphasis, strikethrough, and code voice.

let presentationIntent: AttributeScopes.FoundationAttributes.PresentationIntentAttribute

A property for accessing a presentation intent attribute.

struct PresentationIntent

A type that defines presentation intent for blocks of characters like paragraphs, lists, block quotes, and tables.

