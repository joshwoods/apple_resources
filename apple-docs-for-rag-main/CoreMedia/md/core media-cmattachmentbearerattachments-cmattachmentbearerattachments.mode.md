

- Core Media
- CMAttachmentBearerAttachments
-  CMAttachmentBearerAttachments.Mode 

Enumeration

# CMAttachmentBearerAttachments.Mode

An enumeration that defines the available attachment modes.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum Mode
```

## Topics

### Cases

case shouldPropagate

A mode that propagates attachments.

case shouldNotPropagate

A mode that doesn’t propagate attachments.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Managing Attachments

func merge([String : Any], mode: CMAttachmentBearerAttachments.Mode)

Sets a collection of attachments on the object.

func removeAll()

Removes all attachments from this object.

