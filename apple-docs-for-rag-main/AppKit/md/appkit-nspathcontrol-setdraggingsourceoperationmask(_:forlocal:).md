

- AppKit
- NSPathControl
-  setDraggingSourceOperationMask(\_:forLocal:) 

Instance Method

# setDraggingSourceOperationMask(\_:forLocal:)

Configures the default value returned from draggingSourceOperationMaskForLocal:.

macOS 10.5+

``` source
@MainActor
func setDraggingSourceOperationMask(
    _ mask: NSDragOperation,
    forLocal isLocal: Bool
)
```

## Parameters 

`mask`  

The types of drag operations allowed.

`isLocal`  

If true, `mask` applies when the drag destination object is in the same application as the receiver; if false, `mask` applies when the destination object is outside the receiver’s application.

## Discussion

By default, draggingSourceOperationMaskForLocal: returns `NSDragOperationEvery` when `isLocal` is true and `NSDragOperationNone` when `isLocal` is false.

