

- AppKit
- NSSplitView
-  setPosition(\_:ofDividerAt:) 

Instance Method

# setPosition(\_:ofDividerAt:)

Updates the location of a divider you specify by index.

macOS 10.5+

``` source
@MainActor
func setPosition(
    _ position: CGFloat,
    ofDividerAt dividerIndex: Int
)
```

## Parameters 

`position`  

The position of the divider.

`dividerIndex`  

The index of the divider.

## Discussion

One of the views adjacent to the divider may collapse because the method’s default implementation assumes a person is dragging the divider to the new location. The Auto Layout system collapses the view if it can’t satisfy the view’s constraints — typically imposed by its delegate — with the divider’s new location.

NSSplitView doesn’t invoke this method.

## See Also

### Constraining Split Position

func minPossiblePositionOfDivider(at: Int) -> CGFloat

Returns the minimum possible position of the divider at the specified index.

func maxPossiblePositionOfDivider(at: Int) -> CGFloat

Returns the maximum possible position of the divider at the specified index.

