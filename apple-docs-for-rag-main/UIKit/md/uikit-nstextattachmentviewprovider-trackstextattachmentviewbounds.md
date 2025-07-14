

- UIKit
- NSTextAttachmentViewProvider
-  tracksTextAttachmentViewBounds 

Instance Property

# tracksTextAttachmentViewBounds

A Boolean value that determines the text attachment’s bounds policy.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
var tracksTextAttachmentViewBounds: Bool { get set }
```

## Discussion

If `true`, the framework calls the `textAttachment` property’s attachmentBounds(for:location:textContainer:proposedLineFragment:position:) method and examines the text attachment view provider to determine the bounds instead of using the `bounds` property of this instance. Defaults to `false`.

## See Also

### Defining the contents

var location: any NSTextLocation

The location that indicates the start of the text attachment.

var textAttachment: NSTextAttachment?

The text attachment for this view.

var textLayoutManager: NSTextLayoutManager?

The text layout manager for this view.

var view: UIView?

The text attachment’s view.

