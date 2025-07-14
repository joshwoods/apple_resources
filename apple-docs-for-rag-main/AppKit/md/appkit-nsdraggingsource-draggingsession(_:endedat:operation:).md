

- AppKit
- NSDraggingSource
-  draggingSession(\_:endedAt:operation:) 

Instance Method

# draggingSession(\_:endedAt:operation:)

Invoked when the dragging session has completed.

macOS 10.7+

``` source
@MainActor
optional func draggingSession(
    _ session: NSDraggingSession,
    endedAt screenPoint: NSPoint,
    operation: NSDragOperation
)
```

## Parameters 

`session`  

The dragging session.

`screenPoint`  

The point where the drag ended, in screen coordinates.

`operation`  

The drag operation. See NSDragOperation for drag operation types.

## See Also

### Dragging Session Locations

func draggingSession(NSDraggingSession, willBeginAt: NSPoint)

Invoked when the drag will begin.

func draggingSession(NSDraggingSession, movedTo: NSPoint)

Invoked when the drag moves on the screen.

