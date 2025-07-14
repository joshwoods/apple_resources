

- Core Video
-  CVBufferGetAttachments(\_:\_:) Deprecated

Function

# CVBufferGetAttachments(\_:\_:)

Retrieves all attachments of a Core Video buffer.

iOS 4.0–15.0DeprecatediPadOS 4.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.4–12.0DeprecatedtvOS 9.0–15.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 4.0–8.0Deprecated

``` source
func CVBufferGetAttachments(
    _ buffer: CVBuffer,
    _ attachmentMode: CVAttachmentMode
) -> CFDictionary?
```

Deprecated

Use CVBufferCopyAttachments(_:_:) instead.

## Parameters 

`buffer`  

The buffer whose attachments you want to retrieve.

`attachmentMode`  

The mode of the attachments you want to retrieve. See CVAttachmentMode for possible values.

## Return Value

A Core Foundation dictionary with all attachments identified by keys, or nil if the attachment mode is invalid. The dictionary is empty if the buffer has no attachments.

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

func CVBufferGetAttachment(CVBuffer, CFString, UnsafeMutablePointer&lt;CVAttachmentMode>?) -> Unmanaged&lt;CFTypeRef>?

Retrieves a specific attachment of a Core Video buffer.

Deprecated

