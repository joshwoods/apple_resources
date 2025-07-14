

- Core Video
-  CVBufferSetAttachment(\_:\_:\_:\_:) 

Function

# CVBufferSetAttachment(\_:\_:\_:\_:)

Sets or adds an attachment to a Core Video buffer.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CVBufferSetAttachment(
    _ buffer: CVBuffer,
    _ key: CFString,
    _ value: CFTypeRef,
    _ attachmentMode: CVAttachmentMode
)
```

## Parameters 

`buffer`  

The buffer on which to add or set an attachment.

`key`  

A string that identifies the attachment, which can be of any doc://com.apple.documentation/documentation/corefoundation/cftype. See CVBuffer Attachment Keys and Image Buffer Attachment Keys for predefined values.

`value`  

The attachment in the form of a Core Foundation object. If this parameter is `NULL`, the function returns an error.

`attachmentMode`  

The attachment mode for this attachment. See CVAttachmentMode for possible values. Any given attachment key may exist in only one mode at a time.

## Discussion

You can attach any Core Foundation object to a Core Video buffer to store additional information.

If it doesn’t exist for the buffer object, the system adds a new attachment. If the key does exist, the system replaces the existing attachment. In both cases, the system increases the retain count of the attachment.

You can also set attachments when creating a buffer by specifying them in the kCVBufferPropagatedAttachmentsKey or kCVBufferNonPropagatedAttachmentsKey attributes.

To retrieve attachments, use the CVBufferGetAttachment(_:_:_:) or CVBufferGetAttachments(_:_:) functions.

## See Also

### Working with attachments

func CVBufferHasAttachment(CVBuffer, CFString) -> Bool

Returns a Boolean value that indicates whether a Core Video buffer contains a specified attachment.

func CVBufferCopyAttachment(CVBuffer, CFString, UnsafeMutablePointer&lt;CVAttachmentMode>?) -> CFTypeRef?

Returns a copy of an attachment from a Core Video buffer.

func CVBufferCopyAttachments(CVBuffer, CVAttachmentMode) -> CFDictionary?

Returns a copy of all attachments from a Core Video buffer.

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

