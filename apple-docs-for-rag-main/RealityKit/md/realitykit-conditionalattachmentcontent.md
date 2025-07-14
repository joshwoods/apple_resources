

- RealityKit
-  ConditionalAttachmentContent 

Structure

# ConditionalAttachmentContent

RealityKitSwiftUIvisionOS 1.0+

``` source
@frozen
struct ConditionalAttachmentContent
```

## Topics

### Default Implementations

AttachmentContent Implementations

## Relationships

### Conforms To

- AttachmentContent

  Conforms when `TrueContent` conforms to `AttachmentContent` and `FalseContent` conforms to `AttachmentContent`.

- Copyable

## See Also

### Attachment types

struct AttachmentContentBuilder

A result builder that creates attachment content from closures.

protocol AttachmentContent

A type that provides content for an attachment content builder.

struct EmptyAttachmentContent

A attachment content that doesn’t contain any content.

struct TupleAttachmentContent

struct AnyAttachmentContent

A type-erased attachment content.

