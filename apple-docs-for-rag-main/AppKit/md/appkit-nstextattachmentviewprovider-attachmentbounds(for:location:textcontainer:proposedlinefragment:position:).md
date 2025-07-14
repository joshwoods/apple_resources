

- AppKit
- NSTextAttachmentViewProvider
-  attachmentBounds(for:location:textContainer:proposedLineFragment:position:) 

Instance Method

# attachmentBounds(for:location:textContainer:proposedLineFragment:position:)

Returns the layout bounds for an attachment at a specific text location that contains the text attributes you specify.

macOS 12.0+

``` source
func attachmentBounds(
    for attributes: [NSAttributedString.Key : Any],
    location: any NSTextLocation,
    textContainer: NSTextContainer?,
    proposedLineFragment: CGRect,
    position: CGPoint
) -> CGRect
```

## Parameters 

`attributes`  

A dictionary that contains a list of key and attribute pairs that describe the customization of the string.

`location`  

An NSTextLocation that indicates that start of the string.

`textContainer`  

The NSTextContainer that contains the source string.

`proposedLineFragment`  

A CGRect that describes the boundaries of the line fragment.

`position`  

A CGPoint inside `proposedLineFragment`.

## Return Value

Returns a CGRect that describes the bounds of the attachment.

