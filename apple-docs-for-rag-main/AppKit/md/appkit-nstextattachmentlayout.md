

- AppKit
-  NSTextAttachmentLayout 

Protocol

# NSTextAttachmentLayout

A set of methods that defines the interface to attachment objects from a text layout manager.

macOS 12.0+

``` source
protocol NSTextAttachmentLayout : NSObjectProtocol
```

## Overview

`The NSTextAttachmentLayout` protocol is the interface for working with attachment objects with an NSTextAttachmentViewProvider using a NSTextLayoutManager in macOS 12 and iOS 15 and later.

## Topics

### Determining the characteristics of an attachment

func attachmentBounds(for: [NSAttributedString.Key : Any], location: any NSTextLocation, textContainer: NSTextContainer?, proposedLineFragment: CGRect, position: CGPoint) -> CGRect

Returns the layout bounds of the attachment you specify.

**Required**

func image(for: CGRect, attributes: [NSAttributedString.Key : Any], location: any NSTextLocation, textContainer: NSTextContainer?) -> NSImage?

Returns the image object rendered at the bounds and inside the text container you specify.

**Required**

func viewProvider(for: NSView?, location: any NSTextLocation, textContainer: NSTextContainer?) -> NSTextAttachmentViewProvider?

Returns the text attachment view provider corresponding to the file type.

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

protocol NSTextAttachmentContainer

A set of methods that defines the interface to text attachment objects from a layout manager.

class NSTextAttachmentCell

An object that implements the functionality of the text attachment cell protocol.

protocol NSTextAttachmentCellProtocol

A set of methods that declares the interface for objects that draw text attachment icons and handle mouse events on their icons.

