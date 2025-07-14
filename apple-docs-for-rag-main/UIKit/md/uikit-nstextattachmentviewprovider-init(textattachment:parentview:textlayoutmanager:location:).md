

- UIKit
- NSTextAttachmentViewProvider
-  init(textAttachment:parentView:textLayoutManager:location:) 

Initializer

# init(textAttachment:parentView:textLayoutManager:location:)

Creates a new text attachment view whose content starts at the location you provide.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
init(
    textAttachment: NSTextAttachment,
    parentView: UIView?,
    textLayoutManager: NSTextLayoutManager?,
    location: any NSTextLocation
)
```

## Parameters 

`textAttachment`  

The NSTextAttachment for this view.

`parentView`  

The parent view of this attachment.

`textLayoutManager`  

The NSTextLayoutManager for this view.

`location`  

The NSTextLocation that identifies the start of the text.

