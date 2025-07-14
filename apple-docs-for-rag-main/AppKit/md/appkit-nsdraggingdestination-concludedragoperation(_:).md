

- AppKit
- NSDraggingDestination
-  concludeDragOperation(\_:) 

Instance Method

# concludeDragOperation(\_:)

Invoked when the dragging operation is complete, signaling the receiver to perform any necessary clean-up.

macOS

``` source
@MainActor
optional func concludeDragOperation(_ sender: (any NSDraggingInfo)?)
```

## Parameters 

`sender`  

The object sending the message; use it to get details about the dragging operation.

## Discussion

For this method to be invoked, the previous performDragOperation(_:) must have returned true.

The destination implements this method to perform any tidying up that it needs to do, such as updating its visual representation now that it has incorporated the dragged data. This message is the last message sent from `sender` to the destination during a dragging session.

If the `sender` object’s animatesToDestination property was set to true in prepareForDragOperation(_:), then the drag image is still visible. At this point you should draw the final visual representation in the view. When this method returns, the drag image is removed form the screen. If your final visual representation matches the visual representation in the drag, this is a seamless transition.

## See Also

### Managing a Dragging Session After an Image Is Released

func prepareForDragOperation(any NSDraggingInfo) -> Bool

Invoked when the image is released, allowing the receiver to agree to or refuse drag operation.

func performDragOperation(any NSDraggingInfo) -> Bool

Invoked after the released image has been removed from the screen, signaling the receiver to import the pasteboard data.

