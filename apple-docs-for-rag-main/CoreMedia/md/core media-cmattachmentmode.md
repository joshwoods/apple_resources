

- Core Media
-  CMAttachmentMode 

Type Alias

# CMAttachmentMode

The mode to use when propagating attachments.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
typealias CMAttachmentMode = UInt32
```

## Discussion

Set these attributes when adding attachments to a CMAttachmentBearer object.

## Topics

### Modes

var kCMAttachmentMode_ShouldNotPropagate: CMAttachmentMode

A mode that doesn’t propagate attachments to another object.

var kCMAttachmentMode_ShouldPropagate: CMAttachmentMode

A mode that propagates attachments to another object.

## See Also

### Data Types

protocol CMAttachmentBearerProtocol

A protocol for objects that can carry attachments.

typealias CMAttachmentBearer

An object that can carry attachments.

