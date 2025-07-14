

- Core Video
- CVAttachmentMode
-  CVAttachmentMode.shouldPropagate 

Case

# CVAttachmentMode.shouldPropagate

Indicates to copy the attachment.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 4.0+

``` source
case shouldPropagate
```

## Discussion

The CVBufferPropagateAttachments(_:_:) function propagates all attachments that have this attachment mode. For example, in most cases, you’ll want to propagate an attachment bearing a timestamp to each successive buffer.

## See Also

### Constants

case shouldNotPropagate

Indicates to not propagate the attachment.

