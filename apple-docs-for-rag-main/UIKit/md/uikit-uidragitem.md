

- UIKit
-  UIDragItem 

Class

# UIDragItem

A representation of an underlying data item as a person drags it from one location to another.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class UIDragItem
```

## Mentioned in 

Supporting drag and drop in table views

Supporting Drag and Drop in Collection Views

## Topics

### Initializing a drag item

init(itemProvider: NSItemProvider)

Initializes a new drag item with a specified item provider.

### Accessing the drag item’s data

var itemProvider: NSItemProvider

The item provider associated with the drag item.

var localObject: Any?

A custom object associated with the drag item.

### Changing the drag item preview

var previewProvider: (() -> UIDragPreview?)?

A visual preview of the drag item, displayed while the user drags the item across the screen.

func setNeedsDropPreviewUpdate()

Notifies the operating system that an updated drop preview is available for the item.

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

### Drag sources

protocol UIDragDropSession

The common interface for querying the state of both drag sessions and drop sessions.

protocol UIDragSession

The interface for configuring a drag session.

protocol UIDragAnimating

The interface for providing custom animation alongside the system’s lift, drop, and cancellation animations.

