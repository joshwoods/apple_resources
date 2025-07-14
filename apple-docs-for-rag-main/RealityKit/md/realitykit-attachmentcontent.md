

- RealityKit
-  AttachmentContent 

Protocol

# AttachmentContent

A type that provides content for an attachment content builder.

RealityKitSwiftUIvisionOS 1.0+

``` source
@MainActor @preconcurrency
protocol AttachmentContent
```

## Topics

### Associated Types

associatedtype Body : AttachmentContent

**Required**

### Instance Properties

var body: Self.Body

**Required**

## Relationships

### Conforming Types

- AnyAttachmentContent
- Attachment

  Conforms when `Content` conforms to `View`.

- ConditionalAttachmentContent

  Conforms when `TrueContent` conforms to `AttachmentContent` and `FalseContent` conforms to `AttachmentContent`.

- EmptyAttachmentContent
- TupleAttachmentContent

## See Also

### Attachment types

struct AttachmentContentBuilder

A result builder that creates attachment content from closures.

struct ConditionalAttachmentContent

struct EmptyAttachmentContent

A attachment content that doesn’t contain any content.

struct TupleAttachmentContent

struct AnyAttachmentContent

A type-erased attachment content.

