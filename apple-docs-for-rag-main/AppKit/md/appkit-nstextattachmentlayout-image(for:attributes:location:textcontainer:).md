

- AppKit
- NSTextAttachmentLayout
-  image(for:attributes:location:textContainer:) 

Instance Method

# image(for:attributes:location:textContainer:)

Returns the image object rendered at the bounds and inside the text container you specify.

macOS 12.0+

``` source
func image(
    for bounds: CGRect,
    attributes: [NSAttributedString.Key : Any] = [:],
    location: any NSTextLocation,
    textContainer: NSTextContainer?
) -> NSImage?
```

**Required**

## Parameters 

`bounds`  

The CGRect that presents the image boundaries inside `textContainer`.

`attributes`  

A dictionary of NSAttributedString.Key attributes.

`location`  

An NSTextLocation that indicates that start of the string.

`textContainer`  

The NSTextContainer that contains the source text.

## Return Value

An optional image object.

## Discussion

A custom implementation should return an image appropriate for the target rendering context that you derive by arguments to this method. The default NSTextAttachment implementation returns the contents of the `image` property when non-`nil`. If the `image` property is `nil`, it returns an image based on the `contents` and `fileType` properties.

## See Also

### Determining the characteristics of an attachment

func attachmentBounds(for: [NSAttributedString.Key : Any], location: any NSTextLocation, textContainer: NSTextContainer?, proposedLineFragment: CGRect, position: CGPoint) -> CGRect

Returns the layout bounds of the attachment you specify.

**Required**

func viewProvider(for: NSView?, location: any NSTextLocation, textContainer: NSTextContainer?) -> NSTextAttachmentViewProvider?

Returns the text attachment view provider corresponding to the file type.

**Required**

