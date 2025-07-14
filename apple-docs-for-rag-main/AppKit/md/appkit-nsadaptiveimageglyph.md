

- AppKit
-  NSAdaptiveImageGlyph 

Class

# NSAdaptiveImageGlyph

A data object for an emoji-like image that can appear in attributed text.

macOS 15.0+

``` source
class NSAdaptiveImageGlyph
```

## Overview

An NSAdaptiveImageGlyph contains an image that automatically adapts to different sizes and resolutions. The text system creates instances of this type to represent custom emojis that people create using the system interfaces. This type manages multiple images, along with metadata describing how to adapt those images correctly to different fonts and font attributes.

Typically, you receive new NSAdaptiveImageGlyph objects only from the text-input system. When someone creates a new emoji and inserts it into their text, TextKit creates an instance of this type to represent it. If your app examines or changes the attributes of attributed strings, preserve the adaptiveImageGlyph attribute when making any changes. For example, if you filter unknown attributes in a custom text-storage object, update your code to preserve this attribute. The value of the attribute is an NSAdaptiveImageGlyph containing the emoji data. You can save the image data with the rest of your content and use the data to recreate the type later.

## Topics

### Creating an adaptive image glyph

init(imageContent: Data)

Create an adaptive image glyph from the previously saved data.

init(coder: NSCoder)

### Getting the image data

var imageContent: Data

The raw data for the image.

### Getting the content metadata

var contentIdentifier: String

A unique identifier for this image.

var contentDescription: String

An alternate textual description of the image contents.

class var contentType: UTType

The image data format to use for this image type.

### Initializers

convenience init(AttributedString.AdaptiveImageGlyph)

## Relationships

### Inherits From

- NSObject

### Conforms To

- CTAdaptiveImageProviding
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Attachments

class NSTextAttachment

The values for the attachment characteristics of attributed strings and related objects.

class NSTextAttachmentViewProvider

A container object that associates a text attachment at a particular document location with a view object.

protocol NSTextAttachmentContainer

A set of methods that defines the interface to text attachment objects from a layout manager.

protocol NSTextAttachmentLayout

A set of methods that defines the interface to attachment objects from a text layout manager.

class NSTextAttachmentCell

An object that implements the functionality of the text attachment cell protocol.

protocol NSTextAttachmentCellProtocol

A set of methods that declares the interface for objects that draw text attachment icons and handle mouse events on their icons.

