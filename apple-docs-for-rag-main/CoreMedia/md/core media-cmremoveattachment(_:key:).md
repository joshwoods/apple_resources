

- Core Media
-  CMRemoveAttachment(\_:key:) 

Function

# CMRemoveAttachment(\_:key:)

Removes a specific attachment from an attachment bearer object.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMRemoveAttachment(
    _ target: CMAttachmentBearer,
    key: CFString
)
```

## Parameters 

`target`  

The `CMAttachmentBearer` containing the attachment to remove.

`key`  

Key in the form of a Core Foundation string identifying the desired attachment.

## Discussion

If the attachment exists, the function removes the attachment and decrements the retain count. Given a CVBuffer, `CMRemoveAttachment` is equivalent to `CVBufferRemoveAttachment`.

## See Also

### Processing Attachments

func CMGetAttachment(CMAttachmentBearer, key: CFString, attachmentModeOut: UnsafeMutablePointer&lt;CMAttachmentMode>?) -> CFTypeRef?

Returns an attachment from an attachment bearer object.

func CMCopyDictionaryOfAttachments(allocator: CFAllocator?, target: CMAttachmentBearer, attachmentMode: CMAttachmentMode) -> CFDictionary?

Returns a dictionary of all attachments for an attachment bearer object.

func CMSetAttachment(CMAttachmentBearer, key: CFString, value: CFTypeRef?, attachmentMode: CMAttachmentMode)

Sets or adds an attachment to an attachment bearer object.

func CMSetAttachments(CMAttachmentBearer, attachments: CFDictionary, attachmentMode: CMAttachmentMode)

Sets a dictionary of attachments on an attachment bearer object.

func CMRemoveAllAttachments(CMAttachmentBearer)

Removes all attachments from an attachment bearer object.

func CMPropagateAttachments(CMAttachmentBearer, destination: CMAttachmentBearer)

Copies all propagable attachments from one attachment bearer object to another.

