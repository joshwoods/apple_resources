

- Core Video
-  CVBufferCopyAttachment(\_:\_:\_:) 

Function

# CVBufferCopyAttachment(\_:\_:\_:)

Returns a copy of an attachment from a Core Video buffer.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func CVBufferCopyAttachment(
    _ buffer: CVBuffer,
    _ key: CFString,
    _ attachmentMode: UnsafeMutablePointer?
) -> CFTypeRef?
```

## Parameters 

`buffer`  

A buffer with an attachment to copy.

`key`  

A string that identifies the attachment, which can be of any doc://com.apple.documentation/documentation/corefoundation/cftype. See CVBuffer Attachment Keys and Image Buffer Attachment Keys for predefined values.

`attachmentMode`  

On output, this value points to the mode of the attachment. See CVAttachmentMode for possible values. This value is nil if the buffer doesn’t define an attachment mode.

## Return Value

The requested attachment, or `nil` if no attachment for the specified key exists.

## Discussion

This function returns a retained attachment value, which you need to release when you’re done with it.

## See Also

### Working with attachments

func CVBufferHasAttachment(CVBuffer, CFString) -> Bool

Returns a Boolean value that indicates whether a Core Video buffer contains a specified attachment.

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

func CVBufferRemoveAllAttachments(CVBuffer)

Removes all attachments from a Core Video buffer.

func CVBufferGetAttachment(CVBuffer, CFString, UnsafeMutablePointer&lt;CVAttachmentMode>?) -> Unmanaged&lt;CFTypeRef>?

Retrieves a specific attachment of a Core Video buffer.

Deprecated

func CVBufferGetAttachments(CVBuffer, CVAttachmentMode) -> CFDictionary?

Retrieves all attachments of a Core Video buffer.

Deprecated

