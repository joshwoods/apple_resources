

- UIKit
- UIAttachmentBehavior
-  items 

Instance Property

# items

The dynamic items connected by the attachment behavior.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var items: [any UIDynamicItem] { get }
```

## Discussion

Contains two elements when used for an attachment behavior of type UIAttachmentBehavior.AttachmentType.items; contains one element when used for an attachment behavior of type UIAttachmentBehavior.AttachmentType.anchor.

