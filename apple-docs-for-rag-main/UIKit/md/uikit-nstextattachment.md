

- UIKit
-  NSTextAttachment 

Class

# NSTextAttachment

The values for the attachment characteristics of attributed strings and related objects.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSTextAttachment
```

## Overview

The NSAttributedString class uses text attachment objects as the values for attachment attributes (stored in the attributed string under the attachment key in Swift or the NSAttachmentAttributeName key in Objective-C).

A text attachment object contains either an NSData object or an FileWrapper object, which in turn holds the contents of the attached file. The properties of this class configure the appearance of the text attachment in your interface. In macOS, the text attachment also uses a cell object that conforms to the NSTextAttachmentCellProtocol protocol to draw the image that represents the text and handles mouse events. For more information about text attachments, see the NSAttributedString and NSTextView.

In macOS 12 and iOS 15 and later, NSTextAttachmentViewProvider and NSTextAttachmentLayout provide additional capabilities to represent document locations in terms of an NSTextLocation or an NSTextRange, and provide support for view-based text attachments.

## Topics

### Initializing a text attachment

convenience init(fileWrapper: FileWrapper?)

Creates a text attachment object to contain the specified file wrapper.

init(data: Data?, ofType: String?)

Creates a text attachment object with the specified data.

init(image: UIImage)

Creates a text attachment object to contain the specified image.

### Defining the attachment’s contents

var bounds: CGRect

The layout bounds of the text attachment’s graphical representation in the text coordinate system.

var contents: Data?

The contents for the text attachment.

var fileType: String?

The file type of the contents for the text attachment.

var image: UIImage?

An instance of the relevant image class that represents the contents of the text attachment object.

var fileWrapper: FileWrapper?

The text attachment’s file wrapper.

var allowsTextAttachmentView: Bool

A Boolean value that determines whether the text attachment uses text attachment views.

var usesTextAttachmentView: Bool

A Boolean value that indicates whether the text attachment uses text attachment views.

var lineLayoutPadding: CGFloat

The layout padding before and after the text attachment bounds.

### Setting the attachment cell

var attachmentCell: (any NSTextAttachmentCellProtocol)? { get set }

The object that draws the icon for the text attachment and handles mouse events.

### Constants

class var character: Int

Specifies a character that denotes an attachment.

### Convenience methods

class func registerViewProviderClass(AnyClass, forFileType: String)

Registers a specific file type with the attachment view provider.

class func textAttachmentViewProviderClass(forFileType: String) -> AnyClass?

Returns the text attachment view provider class, if any, for the file type you specify.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding
- NSTextAttachmentContainer
- NSTextAttachmentLayout
- UIAccessibilityContentSizeCategoryImageAdjusting

## See Also

### Attachments

class NSTextAttachmentViewProvider

A container object that associates a text attachment at a particular document location with a view object.

class NSAdaptiveImageGlyph

A data object for an emoji-like image that can appear in attributed text.

protocol NSTextAttachmentContainer

A set of methods that defines the interface to text attachment objects from a layout manager.

protocol NSTextAttachmentLayout

A set of methods that defines the interface to attachment objects from a text layout manager.

