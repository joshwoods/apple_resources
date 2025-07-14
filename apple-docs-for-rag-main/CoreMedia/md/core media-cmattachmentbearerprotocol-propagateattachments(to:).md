

- Core Media
- CMAttachmentBearerProtocol
-  propagateAttachments(to:) 

Instance Method

# propagateAttachments(to:)

Copies all propagable attachments from one attachment bearer object to another.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func propagateAttachments(to destination: T) where T : CMAttachmentBearerProtocol
```

**Required**

## Parameters 

`destination`  

The object to copy attachments to.

## See Also

### Processing Attachments

var attachments: CMAttachmentBearerAttachments

All attachments for this object.

**Required**

struct CMAttachmentBearerAttachments

A structure that contains attachments.

