

- AppKit
- NSDraggingSource
-  draggingSession(\_:movedTo:) 

Instance Method

# draggingSession(\_:movedTo:)

Invoked when the drag moves on the screen.

macOS 10.7+

``` source
@MainActor
optional func draggingSession(
    _ session: NSDraggingSession,
    movedTo screenPoint: NSPoint
)
```

## Parameters 

`session`  

The dragging session.

`screenPoint`  

The point where the drag moved to, in screen coordinates.

## See Also

### Dragging Session Locations

func draggingSession(NSDraggingSession, willBeginAt: NSPoint)

Invoked when the drag will begin.

func draggingSession(NSDraggingSession, endedAt: NSPoint, operation: NSDragOperation)

Invoked when the dragging session has completed.

