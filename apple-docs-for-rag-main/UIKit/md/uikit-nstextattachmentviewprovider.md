

- UIKit
-  NSTextAttachmentViewProvider 

Class

# NSTextAttachmentViewProvider

A container object that associates a text attachment at a particular document location with a view object.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
class NSTextAttachmentViewProvider
```

## Overview

Use `NSTextAttachmentViewProvider` when you need to represent document locations in terms of an NSTextLocation or an NSTextRange or you want to support view-based text attachments. The view provider controls the view placement and layout without requiring view classes to be aware of the text attachment coordination using a NSTextLayoutManager in macOS 12 or iOS 15 and later.

## Topics

### Initializing a text attachment view

init(textAttachment: NSTextAttachment, parentView: UIView?, textLayoutManager: NSTextLayoutManager?, location: any NSTextLocation)

Creates a new text attachment view whose content starts at the location you provide.

### Defining the contents

var location: any NSTextLocation

The location that indicates the start of the text attachment.

var textAttachment: NSTextAttachment?

The text attachment for this view.

var textLayoutManager: NSTextLayoutManager?

The text layout manager for this view.

var tracksTextAttachmentViewBounds: Bool

A Boolean value that determines the text attachment’s bounds policy.

var view: UIView?

The text attachment’s view.

### Defining a custom view hierarchy

func loadView()

Draws the custom view hierarchy that text attachment view subclasses implement.

### Determining the Attachment’s Bounds

func attachmentBounds(for: [NSAttributedString.Key : Any], location: any NSTextLocation, textContainer: NSTextContainer?, proposedLineFragment: CGRect, position: CGPoint) -> CGRect

Returns the layout bounds for an attachment at a specific text location that contains the text attributes you specify.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Attachments

class NSTextAttachment

The values for the attachment characteristics of attributed strings and related objects.

class NSAdaptiveImageGlyph

A data object for an emoji-like image that can appear in attributed text.

protocol NSTextAttachmentContainer

A set of methods that defines the interface to text attachment objects from a layout manager.

protocol NSTextAttachmentLayout

A set of methods that defines the interface to attachment objects from a text layout manager.

