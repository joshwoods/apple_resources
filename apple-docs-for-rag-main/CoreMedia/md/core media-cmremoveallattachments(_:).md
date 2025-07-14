

- Core Media
-  CMRemoveAllAttachments(\_:) 

Function

# CMRemoveAllAttachments(\_:)

Removes all attachments from an attachment bearer object.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMRemoveAllAttachments(_ target: CMAttachmentBearer)
```

## Parameters 

`target`  

The `CMAttachmentBearer` whose attachment you want to remove.

## Discussion

While `CMRemoveAttachment` removes a specific attachment identified by a key, `CMRemoveAllAttachments` removes all attachments of a `CMAttachmentBearer` and decrements their retain counts. Given a CVBuffer, `CMRemoveAllAttachments` is equivalent to `CVBufferRemoveAllAttachments`.

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

func CMPropagateAttachments(CMAttachmentBearer, destination: CMAttachmentBearer)

Copies all propagable attachments from one attachment bearer object to another.

