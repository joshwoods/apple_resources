

- AppKit
- NSDraggingDestination
-  prepareForDragOperation(\_:) 

Instance Method

# prepareForDragOperation(\_:)

Invoked when the image is released, allowing the receiver to agree to or refuse drag operation.

macOS

``` source
@MainActor
optional func prepareForDragOperation(_ sender: any NSDraggingInfo) -> Bool
```

## Parameters 

`sender`  

The object sending the message; use it to get details about the dragging operation.

## Return Value

true if the receiver agrees to perform the drag operation and false if not.

## Discussion

This method is invoked only if the most recent draggingEntered(_:) or draggingUpdated(_:) message returned an acceptable drag-operation value.

If you want the drag items to animate from their current location on screen to their final location in your view, set the sender object’s animatesToDestination property to true in your implementation of this method.

## See Also

### Managing a Dragging Session After an Image Is Released

func performDragOperation(any NSDraggingInfo) -> Bool

Invoked after the released image has been removed from the screen, signaling the receiver to import the pasteboard data.

func concludeDragOperation((any NSDraggingInfo)?)

Invoked when the dragging operation is complete, signaling the receiver to perform any necessary clean-up.

