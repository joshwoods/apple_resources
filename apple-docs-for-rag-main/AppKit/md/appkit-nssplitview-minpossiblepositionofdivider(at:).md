

- AppKit
- NSSplitView
-  minPossiblePositionOfDivider(at:) 

Instance Method

# minPossiblePositionOfDivider(at:)

Returns the minimum possible position of the divider at the specified index.

macOS 10.5+

``` source
@MainActor
func minPossiblePositionOfDivider(at dividerIndex: Int) -> CGFloat
```

## Parameters 

`dividerIndex`  

The index of the divider.

## Return Value

A CGFloat that specifies the minimum possible position of the divider.

## Discussion

The position is *possible* because the bounds of the split view and the current position of other dividers dictate it. *Allowable* positions result from letting the delegate apply constraints to the possible positions.

You can invoke this method to determine the range of values that you can pass to setPosition(_:ofDividerAt:). You can also invoke it from delegate methods like splitView(_:constrainSplitPosition:ofSubviewAt:) to implement relatively complex behaviors that depend on the current state of the split view.

The result of invoking this method when you haven’t invoked adjustSubviews(), and the subview frames are invalid, is undefined.

## See Also

### Constraining Split Position

func maxPossiblePositionOfDivider(at: Int) -> CGFloat

Returns the maximum possible position of the divider at the specified index.

func setPosition(CGFloat, ofDividerAt: Int)

Updates the location of a divider you specify by index.

