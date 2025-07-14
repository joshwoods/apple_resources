

- Foundation
- AttributeScopes
- AttributeScopes.FoundationAttributes
-  AttributeScopes.FoundationAttributes.InlinePresentationIntentAttribute 

Enumeration

# AttributeScopes.FoundationAttributes.InlinePresentationIntentAttribute

A type for using an inline presentation intent as an attribute.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@frozen
enum InlinePresentationIntentAttribute
```

## Overview

An inline presentation intent applies to a run of characters inside a larger block, and covers traits like emphasis, strikethrough, and code voice.

## Relationships

### Conforms To

- AttributedStringKey
- BitwiseCopyable
- Copyable
- DecodableAttributedStringKey
- EncodableAttributedStringKey
- ObjectiveCConvertibleAttributedStringKey

## See Also

### Using presentation intent attributes

let inlinePresentationIntent: AttributeScopes.FoundationAttributes.InlinePresentationIntentAttribute

A property for accessing an inline presentation intent attribute.

struct InlinePresentationIntent

A type that defines presentation intent for runs of characters for traits like emphasis, strikethrough, and code voice.

let presentationIntent: AttributeScopes.FoundationAttributes.PresentationIntentAttribute

A property for accessing a presentation intent attribute.

enum PresentationIntentAttribute

A type for using a presentation intent as an attribute.

struct PresentationIntent

A type that defines presentation intent for blocks of characters like paragraphs, lists, block quotes, and tables.

