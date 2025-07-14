

- Core Video
-  CVBufferRemoveAllAttachments(\_:) 

Function

# CVBufferRemoveAllAttachments(\_:)

Removes all attachments from a Core Video buffer.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CVBufferRemoveAllAttachments(_ buffer: CVBuffer)
```

## Parameters 

`buffer`  

The buffer whose attachments you want to remove.

## Discussion

This function removes all attachments from a buffer and decrements their reference counts.

## See Also

### Working with attachments

func CVBufferHasAttachment(CVBuffer, CFString) -> Bool

Returns a Boolean value that indicates whether a Core Video buffer contains a specified attachment.

func CVBufferCopyAttachment(CVBuffer, CFString, UnsafeMutablePointer&lt;CVAttachmentMode>?) -> CFTypeRef?

Returns a copy of an attachment from a Core Video buffer.

func CVBufferCopyAttachments(CVBuffer, CVAttachmentMode) -> CFDictionary?

Returns a copy of all attachments from a Core Video buffer.

func CVBufferSetAttachment(CVBuffer, CFString, CFTypeRef, CVAttachmentMode)

Sets or adds an attachment to a Core Video buffer.

func CVBufferSetAttachments(CVBuffer, CFDictionary, CVAttachmentMode)

Sets a dictionary of attachments on a Core Video buffer.

func CVBufferPropagateAttachments(CVBuffer, CVBuffer)

Copies all attachments that Core Video can propagate from one buffer to another.

func CVBufferRemoveAttachment(CVBuffer, CFString)

Removes the attachment you specify from a Core Video buffer.

func CVBufferGetAttachment(CVBuffer, CFString, UnsafeMutablePointer&lt;CVAttachmentMode>?) -> Unmanaged&lt;CFTypeRef>?

Retrieves a specific attachment of a Core Video buffer.

Deprecated

func CVBufferGetAttachments(CVBuffer, CVAttachmentMode) -> CFDictionary?

Retrieves all attachments of a Core Video buffer.

Deprecated

