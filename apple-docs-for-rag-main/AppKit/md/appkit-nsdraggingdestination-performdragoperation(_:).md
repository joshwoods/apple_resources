

- AppKit
- NSDraggingDestination
-  performDragOperation(\_:) 

Instance Method

# performDragOperation(\_:)

Invoked after the released image has been removed from the screen, signaling the receiver to import the pasteboard data.

macOS

``` source
@MainActor
optional func performDragOperation(_ sender: any NSDraggingInfo) -> Bool
```

## Parameters 

`sender`  

The object sending the message; use it to get details about the dragging operation.

## Return Value

If the destination accepts the data, it returns true; otherwise it returns false. The default is to return false.

## Discussion

For this method to be invoked, the previous prepareForDragOperation(_:) message must have returned true. The destination should implement this method to do the real work of importing the pasteboard data represented by the image.

If the sender object’s animatesToDestination was set to true in prepareForDragOperation(_:), then setup any animation to arrange space for the drag items to animate to. Also at this time, enumerate through the dragging items to set their destination frames and destination images.

## See Also

### Managing a Dragging Session After an Image Is Released

func prepareForDragOperation(any NSDraggingInfo) -> Bool

Invoked when the image is released, allowing the receiver to agree to or refuse drag operation.

func concludeDragOperation((any NSDraggingInfo)?)

Invoked when the dragging operation is complete, signaling the receiver to perform any necessary clean-up.

