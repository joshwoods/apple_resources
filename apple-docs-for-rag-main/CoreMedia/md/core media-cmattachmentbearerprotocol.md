

- Core Media
-  CMAttachmentBearerProtocol 

Protocol

# CMAttachmentBearerProtocol

A protocol for objects that can carry attachments.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
protocol CMAttachmentBearerProtocol
```

## Topics

### Processing Attachments

var attachments: CMAttachmentBearerAttachments

All attachments for this object.

**Required**

func propagateAttachments&lt;T>(to: T)

Copies all propagable attachments from one attachment bearer object to another.

**Required**

struct CMAttachmentBearerAttachments

A structure that contains attachments.

## Relationships

### Conforming Types

- CMBlockBuffer
- CMSampleBuffer

## See Also

### Data Types

typealias CMAttachmentBearer

An object that can carry attachments.

typealias CMAttachmentMode

The mode to use when propagating attachments.

