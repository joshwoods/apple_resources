

- Core Video
- CVBuffer
-  CVBuffer Attribute Keys 

API Collection

# CVBuffer Attribute Keys

The attributes associated with Core Video buffers.

## Overview

These attributes let you set multiple attachments at the time of buffer creation, rather than having to call CVBufferSetAttachment(_:_:_:_:) for each attachment.

## Topics

### Constants

let kCVBufferPropagatedAttachmentsKey: CFString

Attachments that should be copied when using the CVBufferPropagateAttachments(_:_:) function (type `CFDictionary`, containing a list of attachments as key-value pairs).

let kCVBufferNonPropagatedAttachmentsKey: CFString

Attachments that should not be copied when using the CVBufferPropagateAttachments(_:_:) function (type `CFDictionary`, containing a list of attachments as key-value pairs).

## See Also

### Constants

CVBuffer Attachment Keys

The attachment types for a Core Video buffer.

