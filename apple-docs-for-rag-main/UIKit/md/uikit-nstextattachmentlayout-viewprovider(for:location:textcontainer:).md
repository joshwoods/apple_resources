

- UIKit
- NSTextAttachmentLayout
-  viewProvider(for:location:textContainer:) 

Instance Method

# viewProvider(for:location:textContainer:)

Returns the text attachment view provider corresponding to the file type.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
func viewProvider(
    for parentView: UIView?,
    location: any NSTextLocation,
    textContainer: NSTextContainer?
) -> NSTextAttachmentViewProvider?
```

**Required**

## Parameters 

`parentView`  

The parent view.

`location`  

An NSTextLocation that indicates that start of the string.

`textContainer`  

The NSTextContainer that contains the source text.

## Return Value

An NSTextAttachmentViewProvider.

## Discussion

The default implementation queries the text attachment view provider class using the textAttachmentViewProviderClass(forFileType:) method of NSTextAttachment. When non-`nil`, it instantiates a view, then, fills properties declared in `NSTextAttachmentViewProvider` if implemented.

## See Also

### Determining the characteristics of an attachment

func attachmentBounds(for: [NSAttributedString.Key : Any], location: any NSTextLocation, textContainer: NSTextContainer?, proposedLineFragment: CGRect, position: CGPoint) -> CGRect

Returns the layout bounds of the attachment you specify.

**Required**

func image(for: CGRect, attributes: [NSAttributedString.Key : Any], location: any NSTextLocation, textContainer: NSTextContainer?) -> UIImage?

Returns the image object rendered at the bounds and inside the text container you specify.

**Required**

