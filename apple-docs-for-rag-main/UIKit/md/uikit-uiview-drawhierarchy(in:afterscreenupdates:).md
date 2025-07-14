

- UIKit
- UIView
-  drawHierarchy(in:afterScreenUpdates:) 

Instance Method

# drawHierarchy(in:afterScreenUpdates:)

Renders a snapshot of the complete view hierarchy as visible onscreen into the current context.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func drawHierarchy(
    in rect: CGRect,
    afterScreenUpdates afterUpdates: Bool
) -> Bool
```

## Parameters 

`rect`  

A rectangle specified in the local coordinate system (bounds) of the view.

`afterUpdates`  

A Boolean value that indicates whether the snapshot should be rendered after recent changes have been incorporated. Specify the value false if you want to render a snapshot in the view hierarchy’s current state, which might not include recent changes.

## Return Value

Returns true if the snapshot is complete, or false if the snapshot is missing image data for any view in the hierarchy.

## Discussion

Use this method when you want to apply a graphical effect, such as a blur, to a view snapshot. This method is not as fast as the snapshotView(afterScreenUpdates:) method.

## See Also

### Capturing a view snapshot

func snapshotView(afterScreenUpdates: Bool) -> UIView?

Returns a snapshot view based on the contents of the current view.

func resizableSnapshotView(from: CGRect, afterScreenUpdates: Bool, withCapInsets: UIEdgeInsets) -> UIView?

Returns a snapshot view based on the specified contents of the current view, with stretchable insets.

