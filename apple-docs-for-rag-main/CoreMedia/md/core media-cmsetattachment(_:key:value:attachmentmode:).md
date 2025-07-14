

- Core Media
-  CMSetAttachment(\_:key:value:attachmentMode:) 

Function

# CMSetAttachment(\_:key:value:attachmentMode:)

Sets or adds an attachment to an attachment bearer object.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMSetAttachment(
    _ target: CMAttachmentBearer,
    key: CFString,
    value: CFTypeRef?,
    attachmentMode: CMAttachmentMode
)
```

## Parameters 

`target`  

The `CMAttachmentBearer` object on which to add or set attachments.

`key`  

A `CFString` key identifying the desired attachment.

`value`  

A Core Foundation object attachment. If this parameter is `NULL`, the function returns an error.

`attachmentMode`  

Specifies the attachment mode for this attachment. Any given attachment key may exist in only one mode at a time.

## Discussion

You can attach any Core Foundation object to a `CMAttachmentBearer` object to store additional information. `CMSetAttachment` stores an attachment identified by a key. If the key doesn’t currently exist for the `CMAttachmentBearer` object when you call this function, the function adds the new attachment. If the key does exist, the function replaces the existing attachment. In both cases the function increments the retain count of the attachment. The value can be any `CFType` but a `NULL` value results in an error. Given a CVBuffer, `CMSetAttachment` is equivalent to `CVBufferSetAttachment`.

## See Also

### Processing Attachments

func CMGetAttachment(CMAttachmentBearer, key: CFString, attachmentModeOut: UnsafeMutablePointer&lt;CMAttachmentMode>?) -> CFTypeRef?

Returns an attachment from an attachment bearer object.

func CMCopyDictionaryOfAttachments(allocator: CFAllocator?, target: CMAttachmentBearer, attachmentMode: CMAttachmentMode) -> CFDictionary?

Returns a dictionary of all attachments for an attachment bearer object.

func CMSetAttachments(CMAttachmentBearer, attachments: CFDictionary, attachmentMode: CMAttachmentMode)

Sets a dictionary of attachments on an attachment bearer object.

func CMRemoveAttachment(CMAttachmentBearer, key: CFString)

Removes a specific attachment from an attachment bearer object.

func CMRemoveAllAttachments(CMAttachmentBearer)

Removes all attachments from an attachment bearer object.

func CMPropagateAttachments(CMAttachmentBearer, destination: CMAttachmentBearer)

Copies all propagable attachments from one attachment bearer object to another.

