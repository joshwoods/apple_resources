

- UIKit
-  UITextDragRequest 

Protocol

# UITextDragRequest

The interface for describing the attributes of a drag activity originating in a text view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
protocol UITextDragRequest : NSObjectProtocol
```

## Topics

### Getting the drag items

var existingItems: [UIDragItem]

The array of drag items present in a drag session.

**Required**

var suggestedItems: [UIDragItem]

An array of drag items that the system provides when the text drag delegate doesn’t provide custom drag items.

**Required**

### Getting information about the text

var dragRange: UITextRange

A range of text associated with a drag item in an active drag session that originated in a text view.

**Required**

var isSelected: Bool

A Boolean value indicating whether text is selected for dragging.

**Required**

### Getting the drag session

var dragSession: any UIDragSession

The active drag session.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Drag content

class UITextDragPreviewRenderer

Renders previews of text dragged by the user.

