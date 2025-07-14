

- AppKit
- NSDraggingSession
-  draggingLeaderIndex 

Instance Property

# draggingLeaderIndex

The index of the dragging item under the cursor.

macOS 10.7+

``` source
var draggingLeaderIndex: Int { get set }
```

## Discussion

The index is to an element in the array passed as the first parameter to the NSView method beginDraggingSession(with:event:source:).

The default is the NSDraggingItem closest to the `location` field in the event parameter that was passed to the beginDraggingSession(with:event:source:) method.

