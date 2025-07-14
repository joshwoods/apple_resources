

- AppKit
- NSTextAttachmentViewProvider
-  textAttachment 

Instance Property

# textAttachment

The text attachment for this view.

macOS 12.0+

``` source
weak var textAttachment: NSTextAttachment? { get }
```

## Discussion

Specify the value of this property at initialization time using the init(textAttachment:parentView:textLayoutManager:location:) initializer.

## See Also

### Defining the contents

var location: any NSTextLocation

The location that indicates the start of the text attachment.

var textLayoutManager: NSTextLayoutManager?

The text layout manager for this view.

var tracksTextAttachmentViewBounds: Bool

A Boolean value that determines the text attachment’s bounds policy.

var view: NSView?

The text attachment’s view.

