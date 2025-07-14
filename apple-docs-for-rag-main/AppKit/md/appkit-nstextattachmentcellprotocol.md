

- AppKit
-  NSTextAttachmentCellProtocol 

Protocol

# NSTextAttachmentCellProtocol

A set of methods that declares the interface for objects that draw text attachment icons and handle mouse events on their icons.

macOS

``` source
protocol NSTextAttachmentCellProtocol : NSObjectProtocol
```

## Overview

With the exceptions of cellBaselineOffset(), attachment, and attachment, all of these methods are implemented by the NSCell class.For general information on text attachments, see NSAttributedString and NSTextView.

## Topics

### Setting the attachment

var attachment: NSTextAttachment?

Returns the text attachment object that owns the cell.

**Required**

var attachment: NSTextAttachment?

Returns the text attachment object that owns the cell.

**Required**

### Drawing the cell contents

func draw(withFrame: NSRect, in: NSView?)

Draws the cell’s image in the specified rectangle of the currently focused view.

**Required**

func draw(withFrame: NSRect, in: NSView?, characterIndex: Int)

Draws the cell’s image at the specified index point in the view.

**Required**

func draw(withFrame: NSRect, in: NSView?, characterIndex: Int, layoutManager: NSLayoutManager)

Draws the cell’s image using the specified layout manager.

**Required**

func highlight(Bool, withFrame: NSRect, in: NSView?)

Draws the receiver’s image with optional highlighting.

**Required**

### Providing the cell metrics

func cellSize() -> NSSize

Returns the size of the attachment’s icon.

**Required**

func cellBaselineOffset() -> NSPoint

Returns the text position where you draw the attachment cell’s image, relative to the current point established in the glyph layout.

**Required**

func cellFrame(for: NSTextContainer, proposedLineFragment: NSRect, glyphPosition: NSPoint, characterIndex: Int) -> NSRect

Returns the frame of the cell to draw at the specified position in a text container.

**Required**

### Responding to mouse events

func wantsToTrackMouse() -> Bool

Returns a Boolean value that indicates whether the attachment handles mouse events occurring over its image.

**Required**

func wantsToTrackMouse(for: NSEvent, in: NSRect, of: NSView?, atCharacterIndex: Int) -> Bool

Allows an attachment to specify the events for which it tracks the mouse.

**Required**

func trackMouse(with: NSEvent, in: NSRect, of: NSView?, untilMouseUp: Bool) -> Bool

Handles a mouse-down event on the cell’s image, and optionally waits until a mouse-up event

**Required**

func trackMouse(with: NSEvent, in: NSRect, of: NSView?, atCharacterIndex: Int, untilMouseUp: Bool) -> Bool

Handles a mouse-down event on the image at the specified character position.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- NSTextAttachmentCell

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

protocol NSTextAttachmentLayout

A set of methods that defines the interface to attachment objects from a text layout manager.

class NSTextAttachmentCell

An object that implements the functionality of the text attachment cell protocol.

