

- AppKit
- NSTextAttachmentLayout
-  attachmentBounds(for:location:textContainer:proposedLineFragment:position:) 

Instance Method

# attachmentBounds(for:location:textContainer:proposedLineFragment:position:)

Returns the layout bounds of the attachment you specify.

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

**Required**

## Parameters 

`attributes`  

A dictionary of NSAttributedString.Key attributes.

`location`  

An NSTextLocation that indicates that start of the string.

`textContainer`  

The NSTextContainer that contains the source text.

`proposedLineFragment`  

A CGRect that describes the boundaries of the line fragment.

`position`  

A CGPoint inside `proposedLineFragment`.

## Return Value

Returns a CGRect that describes the boundaries of the attachment, or `CGRectZero.`

## Discussion

The framework interprets the bounds origin to match `position` inside `proposedLineFragment`. The default NSTextAttachment implementation returns bounds if the value isn’t equivalent to CGRectZero; otherwise, it derives the bounds value from `image.size`. Conforming objects can implement more sophisticated logic for negotiating the frame size based on the available container space and proposed line fragment rectangle.

## See Also

### Determining the characteristics of an attachment

func image(for: CGRect, attributes: [NSAttributedString.Key : Any], location: any NSTextLocation, textContainer: NSTextContainer?) -> NSImage?

Returns the image object rendered at the bounds and inside the text container you specify.

**Required**

func viewProvider(for: NSView?, location: any NSTextLocation, textContainer: NSTextContainer?) -> NSTextAttachmentViewProvider?

Returns the text attachment view provider corresponding to the file type.

**Required**

