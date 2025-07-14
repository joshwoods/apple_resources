

- AppKit
- NSDraggingSource
-  draggingSession(\_:willBeginAt:) 

Instance Method

# draggingSession(\_:willBeginAt:)

Invoked when the drag will begin.

macOS 10.7+

``` source
@MainActor
optional func draggingSession(
    _ session: NSDraggingSession,
    willBeginAt screenPoint: NSPoint
)
```

## Parameters 

`session`  

The dragging session.

`screenPoint`  

The point where the drag will begin, in screen coordinates.

## See Also

### Dragging Session Locations

func draggingSession(NSDraggingSession, movedTo: NSPoint)

Invoked when the drag moves on the screen.

func draggingSession(NSDraggingSession, endedAt: NSPoint, operation: NSDragOperation)

Invoked when the dragging session has completed.

