

- AppKit
- NSDraggingSource
-  draggingSession(\_:sourceOperationMaskFor:) 

Instance Method

# draggingSession(\_:sourceOperationMaskFor:)

Declares the types of operations the source allows to be performed.

macOS 10.7+

``` source
@MainActor
func draggingSession(
    _ session: NSDraggingSession,
    sourceOperationMaskFor context: NSDraggingContext
) -> NSDragOperation
```

**Required**

## Parameters 

`session`  

The dragging session.

`context`  

The dragging context. See NSDraggingContext for the supported values.

## Return Value

The appropriate dragging operation as defined in

## Discussion

In the future Apple may provide more specific “within” values in the future. To account for this, for unrecognized localities, return the operation mask for the most specific context that you are concerned with. The following code is an example of how to implement this functionality:

```
    switch(context) {
        case NSDraggingContextOutsideApplication:
            return ...
            break;

        case NSDraggingContextWithinApplication:
        default:
            return ...
            break;
    }
```

