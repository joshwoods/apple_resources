

- AppKit
- NSDraggingDestination
-  updateDraggingItemsForDrag(\_:) 

Instance Method

# updateDraggingItemsForDrag(\_:)

Invoked when the dragging images should be changed.

macOS 10.7+

``` source
@MainActor
optional func updateDraggingItemsForDrag(_ sender: (any NSDraggingInfo)?)
```

## Parameters 

`sender`  

The object sending the message; use this object to get details about the dragging operation.

## Discussion

While a destination may change the dragging images at any time, it is recommended to wait until this method is called before updating the dragging images.

This allows the system to delay changing the dragging images until it is likely that the user will drop on this destination. Otherwise, the dragging images will change too often during the drag which would be distracting to the user.

During `enumerateDraggingItemsWithOptions:forView:classes:searchOptions:usingBlock:` you may set non-acceptable drag items images to `nil` to hide them or use the enumeration option of clearNonenumeratedImages If there are items that you hide, then after enumeration, you need to set the numberOfValidItemsForDrop to the number of non-hidden drag items. However, if the valid item count is `0`, then it is better to return NSDragOperationNone from your implementation of draggingEntered(_:) and, or draggingUpdated(_:) instead of hiding all drag items during enumeration.

