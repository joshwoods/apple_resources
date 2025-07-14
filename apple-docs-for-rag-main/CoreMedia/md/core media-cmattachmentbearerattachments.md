

- Core Media
-  CMAttachmentBearerAttachments 

Structure

# CMAttachmentBearerAttachments

A structure that contains attachments.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct CMAttachmentBearerAttachments
```

## Topics

### Inspecting Attachments

var propagated: [String : Any]

A dictionary of attachments to copy when propagating attachments from one object to another.

var nonPropagated: [String : Any]

A dictionary of attachments to not copy when propagating attachments from one object to another.

### Accessing Attachments

subscript(String) -> CMAttachmentBearerAttachments.Value?

Gets the value associated with the specified attachment.

subscript(CMSampleBuffer.AttachmentKey) -> CMAttachmentBearerAttachments.Value?

Gets the value associated with the specified attachment key.

enum Value

An enumeration of attachment values.

### Managing Attachments

func merge([String : Any], mode: CMAttachmentBearerAttachments.Mode)

Sets a collection of attachments on the object.

enum Mode

An enumeration that defines the available attachment modes.

func removeAll()

Removes all attachments from this object.

## See Also

### Processing Attachments

var attachments: CMAttachmentBearerAttachments

All attachments for this object.

**Required**

func propagateAttachments&lt;T>(to: T)

Copies all propagable attachments from one attachment bearer object to another.

**Required**

