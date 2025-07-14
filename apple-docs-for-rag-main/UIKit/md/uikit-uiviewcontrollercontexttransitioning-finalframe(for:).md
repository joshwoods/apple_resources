

- UIKit
- UIViewControllerContextTransitioning
-  finalFrame(for:) 

Instance Method

# finalFrame(for:)

Returns the ending frame rectangle for the specified view controller’s view.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func finalFrame(for vc: UIViewController) -> CGRect
```

**Required**

## Parameters 

`vc`  

The view controller whose frame rectangle you want.

## Return Value

The frame rectangle for the view or CGRectZero if the frame rectangle is not known or the view is not visible.

## Discussion

The rectangle returned by this method represents the size of the corresponding view at the end of the transition. For the view being covered during the presentation, the value returned by this method might be CGRectZero but it might also be a valid frame rectangle.

## See Also

### Getting the transition frame rectangles

func initialFrame(for: UIViewController) -> CGRect

Returns the starting frame rectangle for the specified view controller’s view.

**Required**

