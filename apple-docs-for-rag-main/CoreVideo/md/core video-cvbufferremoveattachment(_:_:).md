

- Core Video
-  CVBufferRemoveAttachment(\_:\_:) 

Function

# CVBufferRemoveAttachment(\_:\_:)

Removes the attachment you specify from a Core Video buffer.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CVBufferRemoveAttachment(
    _ buffer: CVBuffer,
    _ key: CFString
)
```

## Parameters 

`buffer`  

The buffer containing the attachment to remove.

`key`  

A string that identifies the attachment, which can be of any doc://com.apple.documentation/documentation/corefoundation/cftype. See CVBuffer Attachment Keys and Image Buffer Attachment Keys for predefined values.

## Discussion

If the attachment exists in the buffer, the system removes it and decrements the retain count.

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

func CVBufferRemoveAllAttachments(CVBuffer)

Removes all attachments from a Core Video buffer.

func CVBufferGetAttachment(CVBuffer, CFString, UnsafeMutablePointer&lt;CVAttachmentMode>?) -> Unmanaged&lt;CFTypeRef>?

Retrieves a specific attachment of a Core Video buffer.

Deprecated

func CVBufferGetAttachments(CVBuffer, CVAttachmentMode) -> CFDictionary?

Retrieves all attachments of a Core Video buffer.

Deprecated

