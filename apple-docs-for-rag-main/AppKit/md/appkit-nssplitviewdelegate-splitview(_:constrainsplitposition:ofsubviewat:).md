

- AppKit
- NSSplitViewDelegate
-  splitView(\_:constrainSplitPosition:ofSubviewAt:) 

Instance Method

# splitView(\_:constrainSplitPosition:ofSubviewAt:)

Allows the delegate to constrain the divider to certain positions.

macOS 10.0+

``` source
@MainActor
optional func splitView(
    _ splitView: NSSplitView,
    constrainSplitPosition proposedPosition: CGFloat,
    ofSubviewAt dividerIndex: Int
) -> CGFloat
```

## Parameters 

`splitView`  

The split view that sends the message.

`proposedPosition`  

The cursor’s current position, and the proposed position of the divider.

`dividerIndex`  

The index of the divider the user is moving, with the first divider being `0` and increasing from top to bottom (or left to right).

## Return Value

The position for constraining the divider.

## Discussion

If the delegate implements this method, the split view calls it repeatedly as the user moves the divider.

If a subview’s height must be a multiple of a certain number, use this method to return the multiple nearest to `proposedPosition`.

