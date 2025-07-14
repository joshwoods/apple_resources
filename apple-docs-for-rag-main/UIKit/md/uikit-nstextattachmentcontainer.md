

- UIKit
-  NSTextAttachmentContainer 

Protocol

# NSTextAttachmentContainer

A set of methods that defines the interface to text attachment objects from a layout manager.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
protocol NSTextAttachmentContainer : NSObjectProtocol
```

## Topics

### Getting the bounds

func attachmentBounds(for: NSTextContainer?, proposedLineFragment: CGRect, glyphPosition: CGPoint, characterIndex: Int) -> CGRect

Returns the layout bounds of the text attachment to the layout manager.

**Required**

### Getting the image

func image(forBounds: CGRect, textContainer: NSTextContainer?, characterIndex: Int) -> UIImage?

Returns the image object that the layout manager renders in the specified image bounds rectangle inside the text container.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- NSTextAttachment

## See Also

### Attachments

class NSTextAttachment

The values for the attachment characteristics of attributed strings and related objects.

class NSTextAttachmentViewProvider

A container object that associates a text attachment at a particular document location with a view object.

class NSAdaptiveImageGlyph

A data object for an emoji-like image that can appear in attributed text.

protocol NSTextAttachmentLayout

A set of methods that defines the interface to attachment objects from a text layout manager.

