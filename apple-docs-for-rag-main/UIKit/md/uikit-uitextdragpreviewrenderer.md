

- UIKit
-  UITextDragPreviewRenderer 

Class

# UITextDragPreviewRenderer

Renders previews of text dragged by the user.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class UITextDragPreviewRenderer
```

## Overview

Use this class to provide custom previews of dragged text that follows user interface guidelines and handles right-to-left text. You provide the layout manager and the range to render the preview.

Subclasses may override the adjust(firstLineRect:bodyRect:lastLineRect:textOrigin:) method to modify the detected rectangles as needed during the drag operation.

## Topics

### Initializing a text drag preview renderer

convenience init(layoutManager: NSLayoutManager, range: NSRange)

Initializes and returns a text drag preview renderer with the specified layout managers and range to render the text drag preview.

init(layoutManager: NSLayoutManager, range: NSRange, unifyRects: Bool)

Returns an initialized renderer of a text drag preview with the specified layout manager, range, and rectangle detection behavior.

### Getting and setting bounding rectangles

var bodyRect: CGRect

The bounding rectangle of the text in the middle of the drag preview.

var firstLineRect: CGRect

The bounding rectangle of the first line of text in the drag preview.

var lastLineRect: CGRect

The bounding rectangle of the last line of text in the drag preview.

func adjust(firstLineRect: UnsafeMutablePointer&lt;CGRect>, bodyRect: UnsafeMutablePointer&lt;CGRect>, lastLineRect: UnsafeMutablePointer&lt;CGRect>, textOrigin: CGPoint)

Adjusts the size and origin of the bounding rectangles during a text drag operation.

### Getting the preview image

var image: UIImage

The image of the text drag preview that’s rendered by the layout manager.

### Getting the layout manager

var layoutManager: NSLayoutManager

The layout manager that renders the text drag preview.

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
- Sendable

## See Also

### Drag content

protocol UITextDragRequest

The interface for describing the attributes of a drag activity originating in a text view.

