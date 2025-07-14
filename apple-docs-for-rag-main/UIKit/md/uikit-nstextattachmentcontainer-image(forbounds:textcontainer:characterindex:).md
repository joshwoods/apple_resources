

- UIKit
- NSTextAttachmentContainer
-  image(forBounds:textContainer:characterIndex:) 

Instance Method

# image(forBounds:textContainer:characterIndex:)

Returns the image object that the layout manager renders in the specified image bounds rectangle inside the text container.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
func image(
    forBounds imageBounds: CGRect,
    textContainer: NSTextContainer?,
    characterIndex charIndex: Int
) -> UIImage?
```

**Required**

## Parameters 

`imageBounds`  

The rectangle in which the image is laid out.

`textContainer`  

The text container in which the image is laid out.

`charIndex`  

The character location inside the text storage for the attachment character.

## Return Value

The image rendered in the bounds rectangle.

## Discussion

The method should return an image appropriate for the target rendering context derived by arguments passed into this method. The `NSTextAttachment` implementation returns the text attachment’s image when non-`nil`. If the image is `nil`, it returns an image based on the text attachment’s contents and fileType properties.

