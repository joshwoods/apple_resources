

- Core Media
-  CMPropagateAttachments(\_:destination:) 

Function

# CMPropagateAttachments(\_:destination:)

Copies all propagable attachments from one attachment bearer object to another.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMPropagateAttachments(
    _ source: CMAttachmentBearer,
    destination: CMAttachmentBearer
)
```

## Parameters 

`source`  

`CMAttachmentBearer` to copy attachments from.

`destination`  

`CMAttachmentBearer` to copy attachments to.

## Discussion

`CMPropagateAttachments` is a convenience call that copies all attachments with a mode of `kCMAttachmentMode_ShouldPropagate` from one buffer to another. Given a CVBuffer, `CMPropagateAttachments` is equivalent to `CVBufferPropagateAttachments`.

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

func CMRemoveAttachment(CMAttachmentBearer, key: CFString)

Removes a specific attachment from an attachment bearer object.

func CMRemoveAllAttachments(CMAttachmentBearer)

Removes all attachments from an attachment bearer object.

