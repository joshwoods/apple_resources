

- Core Media
-  CMGetAttachment(\_:key:attachmentModeOut:) 

Function

# CMGetAttachment(\_:key:attachmentModeOut:)

Returns an attachment from an attachment bearer object.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMGetAttachment(
    _ target: CMAttachmentBearer,
    key: CFString,
    attachmentModeOut: UnsafeMutablePointer?
) -> CFTypeRef?
```

## Parameters 

`target`  

Specifies the `CMAttachmentBearer` whose attachment you want to retrieve.

`key`  

Key in the form of a `CFString` identifying the desired attachment.

`attachmentModeOut`  

On output, `attachmentMode` points to the mode of the attachment. See CMAttachmentModefor possible values. May be `NULL`.

## Return Value

The requested attachment object or `NULL` if not found.

## Discussion

You can attach any Core Foundation object to a `CMAttachmentBearer` to store additional information. `CMGetAttachment` retrieves an attachment identified by a key. Given a CVBuffer, `CMGetAttachment` is equivalent to CVBufferCopyAttachment(_:_:_:).

## See Also

### Processing Attachments

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

func CMPropagateAttachments(CMAttachmentBearer, destination: CMAttachmentBearer)

Copies all propagable attachments from one attachment bearer object to another.

