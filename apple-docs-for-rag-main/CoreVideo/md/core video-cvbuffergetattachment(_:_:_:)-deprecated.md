

- Core Video
-  CVBufferGetAttachment(\_:\_:\_:) Deprecated

Function

# CVBufferGetAttachment(\_:\_:\_:)

Retrieves a specific attachment of a Core Video buffer.

iOS 4.0–15.0DeprecatediPadOS 4.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.4–12.0DeprecatedtvOS 9.0–15.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 4.0–8.0Deprecated

``` source
func CVBufferGetAttachment(
    _ buffer: CVBuffer,
    _ key: CFString,
    _ attachmentMode: UnsafeMutablePointer?
) -> Unmanaged?
```

Deprecated

Use CVBufferCopyAttachment(_:_:_:) instead.

## Parameters 

`buffer`  

The buffer whose attachment you want to retrieve.

`key`  

A string that identifies the attachment, which can be of any doc://com.apple.documentation/documentation/corefoundation/cftype. See CVBuffer Attachment Keys and Image Buffer Attachment Keys for predefined values.

`attachmentMode`  

On output, this value points to the mode of the attachment. See CVAttachmentMode for possible values. This value is nil if the buffer doesn’t define an attachment mode.

## Return Value

The specified attachment, if it exists.

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

func CVBufferRemoveAllAttachments(CVBuffer)

Removes all attachments from a Core Video buffer.

func CVBufferGetAttachments(CVBuffer, CVAttachmentMode) -> CFDictionary?

Retrieves all attachments of a Core Video buffer.

Deprecated

