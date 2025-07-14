

- Core Media
-  CMCopyDictionaryOfAttachments(allocator:target:attachmentMode:) 

Function

# CMCopyDictionaryOfAttachments(allocator:target:attachmentMode:)

Returns a dictionary of all attachments for an attachment bearer object.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMCopyDictionaryOfAttachments(
    allocator: CFAllocator?,
    target: CMAttachmentBearer,
    attachmentMode: CMAttachmentMode
) -> CFDictionary?
```

## Parameters 

`allocator`  

Allocator for the new dictionary; pass kCFAllocatorDefault or `NULL` to use the default allocator.

`target`  

Specifies the CMAttachmentBearer whose attachments you want to obtain.

`attachmentMode`  

The mode of the attachments you want to obtain. See CMAttachmentMode for possible values.

## Return Value

A Core Foundation dictionary with all attachments identified by their keys. If no attachment is present, the dictionary is empty. Returns `NULL` for an invalid attachment mode.

## Discussion

`CMCopyDictionaryOfAttachments` is a convenience call that returns all attachments with their corresponding keys in a new CFDictionary. Given a `CVBufferRef`, `CMCopyDictionaryOfAttachments` is similar to `CVBufferGetAttachments`, except that the `CFDictionary` that `CMCopyDictionaryOfAttachments` returns isn’t updated for later changes to the attachments.

## See Also

### Processing Attachments

func CMGetAttachment(CMAttachmentBearer, key: CFString, attachmentModeOut: UnsafeMutablePointer&lt;CMAttachmentMode>?) -> CFTypeRef?

Returns an attachment from an attachment bearer object.

func CMSetAttachment(CMAttachmentBearer, key: CFString, value: CFTypeRef?, attachmentMode: CMAttachmentMode)

Sets or adds an attachment to an attachment bearer object.

func CMSetAttachments(CMAttachmentBearer, attachments: CFDictionary, attachmentMode: CMAttachmentMode)

Sets a dictionary of attachments on an attachment bearer object.

func CMRemoveAttachment(CMAttachmentBearer, key: CFString)

Removes a specific attachment from an attachment bearer object.

func CMRemoveAllAttachments(CMAttachmentBearer)

Removes all attachments from an attachment bearer object.

func CMPropagateAttachments(CMAttachmentBearer, destination: CMAttachmentBearer)

Copies all propagable attachments from one attachment bearer object to another.

