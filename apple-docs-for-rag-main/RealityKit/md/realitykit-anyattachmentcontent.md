

- RealityKit
-  AnyAttachmentContent 

Structure

# AnyAttachmentContent

A type-erased attachment content.

RealityKitSwiftUIvisionOS 2.0+

``` source
@MainActor @frozen @preconcurrency
struct AnyAttachmentContent
```

## Overview

An `AnyAttachmentContent` allows changing the type of attachment used in a given attachment content. Whenever the type of attachment content used with an `AnyAttachmentContent` changes, the old content is destroyed and the new content is created for the new type.

## Topics

### Initializers

init&lt;Content>(Content)

Creates an instance that type-erases AttachmentContent.

### Type Aliases

typealias Body

## Relationships

### Conforms To

- AttachmentContent
- Sendable

## See Also

### Attachment types

struct AttachmentContentBuilder

A result builder that creates attachment content from closures.

protocol AttachmentContent

A type that provides content for an attachment content builder.

struct ConditionalAttachmentContent

struct EmptyAttachmentContent

A attachment content that doesn’t contain any content.

struct TupleAttachmentContent

