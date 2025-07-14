

- Core Media
-  CMSetAttachments(\_:attachments:attachmentMode:) 

Function

# CMSetAttachments(\_:attachments:attachmentMode:)

Sets a dictionary of attachments on an attachment bearer object.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMSetAttachments(
    _ target: CMAttachmentBearer,
    attachments theAttachments: CFDictionary,
    attachmentMode: CMAttachmentMode
)
```

## Parameters 

`target`  

The target `CMAttachmentBearer` to set the attachment to.

`theAttachments`  

The attachments to set, in the form of a Core Foundation dictionary.

`attachmentMode`  

Specifies the attachment mode for this attachment. A particular attachment key can only exist in a single mode at a time.

## Discussion

`CMSetAttachments` is a convenience call that in turn calls `CMSetAttachment` for each key and value in the given dictionary. All key value pairs must be in the root level of the dictionary. Given a CVBuffer, `CMSetAttachments` is equivalent to `CVBufferSetAttachments`.

## See Also

### Processing Attachments

func CMGetAttachment(CMAttachmentBearer, key: CFString, attachmentModeOut: UnsafeMutablePointer&lt;CMAttachmentMode>?) -> CFTypeRef?

Returns an attachment from an attachment bearer object.

func CMCopyDictionaryOfAttachments(allocator: CFAllocator?, target: CMAttachmentBearer, attachmentMode: CMAttachmentMode) -> CFDictionary?

Returns a dictionary of all attachments for an attachment bearer object.

func CMSetAttachment(CMAttachmentBearer, key: CFString, value: CFTypeRef?, attachmentMode: CMAttachmentMode)

Sets or adds an attachment to an attachment bearer object.

func CMRemoveAttachment(CMAttachmentBearer, key: CFString)

Removes a specific attachment from an attachment bearer object.

func CMRemoveAllAttachments(CMAttachmentBearer)

Removes all attachments from an attachment bearer object.

func CMPropagateAttachments(CMAttachmentBearer, destination: CMAttachmentBearer)

Copies all propagable attachments from one attachment bearer object to another.

