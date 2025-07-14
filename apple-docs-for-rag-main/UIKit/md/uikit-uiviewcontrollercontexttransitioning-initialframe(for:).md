

- UIKit
- UIViewControllerContextTransitioning
-  initialFrame(for:) 

Instance Method

# initialFrame(for:)

Returns the starting frame rectangle for the specified view controller’s view.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func initialFrame(for vc: UIViewController) -> CGRect
```

**Required**

## Parameters 

`vc`  

The view controller whose frame rectangle you want.

## Return Value

The frame rectangle for the view or CGRectZero if the frame rectangle is not known or the view is not visible.

## Discussion

The rectangle returned by this method represents the size of the corresponding view at the beginning of the transition. For the view controller that is already onscreen, this rectangle typically matches the frame rectangle of the container view. For the view controller being presented, the value returned by this method is typically CGRectZero because the view is not yet on screen.

## See Also

### Getting the transition frame rectangles

func finalFrame(for: UIViewController) -> CGRect

Returns the ending frame rectangle for the specified view controller’s view.

**Required**

