

- UIKit
- NSTextAttachmentViewProvider
-  textLayoutManager 

Instance Property

# textLayoutManager

The text layout manager for this view.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
weak var textLayoutManager: NSTextLayoutManager? { get }
```

## Discussion

Specify the value of this property at initialization time using the init(textAttachment:parentView:textLayoutManager:location:) initializer.

## See Also

### Defining the contents

var location: any NSTextLocation

The location that indicates the start of the text attachment.

var textAttachment: NSTextAttachment?

The text attachment for this view.

var tracksTextAttachmentViewBounds: Bool

A Boolean value that determines the text attachment’s bounds policy.

var view: UIView?

The text attachment’s view.

