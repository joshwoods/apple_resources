

- UIKit
- UITextDragRequest
-  suggestedItems 

Instance Property

# suggestedItems

An array of drag items that the system provides when the text drag delegate doesn’t provide custom drag items.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var suggestedItems: [UIDragItem] { get }
```

**Required**

## Discussion

The suggestedItems property is always an empty array if the text drag delegate doesn’t implement the textDraggableView(_:itemsForDrag:) method.

## See Also

### Getting the drag items

var existingItems: [UIDragItem]

The array of drag items present in a drag session.

**Required**

