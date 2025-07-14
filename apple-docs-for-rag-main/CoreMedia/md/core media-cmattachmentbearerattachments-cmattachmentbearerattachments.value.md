

- Core Media
- CMAttachmentBearerAttachments
-  CMAttachmentBearerAttachments.Value 

Enumeration

# CMAttachmentBearerAttachments.Value

An enumeration of attachment values.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum Value
```

## Topics

### Cases

case shouldPropagate(Any)

A case that indicates to propagate a value.

case shouldNotPropagate(Any)

A case that indicates to not propagate a value.

### Properties

var value: Any

An attachment value.

var mode: CMAttachmentBearerAttachments.Mode

An attachment mode.

## See Also

### Accessing Attachments

subscript(String) -> CMAttachmentBearerAttachments.Value?

Gets the value associated with the specified attachment.

subscript(CMSampleBuffer.AttachmentKey) -> CMAttachmentBearerAttachments.Value?

Gets the value associated with the specified attachment key.

