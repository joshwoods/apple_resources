

- AppKit
- NSTextAttachmentViewProvider
-  init(textAttachment:parentView:textLayoutManager:location:) 

Initializer

# init(textAttachment:parentView:textLayoutManager:location:)

Creates a new text attachment view whose content starts at the location you provide.

macOS 12.0+

``` source
init(
    textAttachment: NSTextAttachment,
    parentView: NSView?,
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

