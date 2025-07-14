

- AppKit
-  NSTextAttachmentCell 

Class

# NSTextAttachmentCell

An object that implements the functionality of the text attachment cell protocol.

macOS

``` source
@MainActor
class NSTextAttachmentCell
```

## Overview

This specification describes only those methods whose implementations have features that are particular to this class. For a general discussion of the protocol’s methods, see NSTextAttachmentCellProtocol.

## Relationships

### Inherits From

- NSCell

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSAccessibilityElementProtocol
- NSAccessibilityProtocol
- NSCoding
- NSCopying
- NSObjectProtocol
- NSTextAttachmentCellProtocol
- NSUserInterfaceItemIdentification
- Sendable

## See Also

### Related Documentation

Text Attachment Programming Topics

### Attachments

class NSTextAttachment

The values for the attachment characteristics of attributed strings and related objects.

class NSTextAttachmentViewProvider

A container object that associates a text attachment at a particular document location with a view object.

class NSAdaptiveImageGlyph

A data object for an emoji-like image that can appear in attributed text.

protocol NSTextAttachmentContainer

A set of methods that defines the interface to text attachment objects from a layout manager.

protocol NSTextAttachmentLayout

A set of methods that defines the interface to attachment objects from a text layout manager.

protocol NSTextAttachmentCellProtocol

A set of methods that declares the interface for objects that draw text attachment icons and handle mouse events on their icons.

