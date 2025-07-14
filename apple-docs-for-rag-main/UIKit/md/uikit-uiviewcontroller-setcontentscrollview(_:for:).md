

- UIKit
- UIViewController
-  setContentScrollView(\_:for:) 

Instance Method

# setContentScrollView(\_:for:)

Sets the scroll view that bars observe for the specified edge.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
@MainActor
func setContentScrollView(
    _ scrollView: UIScrollView?,
    for edge: NSDirectionalRectEdge
)
```

## Parameters 

`scrollView`  

The scroll view to observe. If `nil`, the view controller determines a scroll view automatically.

`edge`  

The edge to observe for scroll view content alignment. Pass top or bottom to set the scroll view for a specific edge, or pass all to set the scroll view for all edges.

## Discussion

Toolbars, navigation bars, and tab bars adjust their appearance when the edge of a scroll view’s content aligns with the edge of the bar. The view controller identifies a scroll view to observe by analyzing the view hierarchy to select a scroll view. If the view hierarchy is complex, the view controller might not select the appropriate scroll view to observe. Use this method to indicate a specific scroll view for the view controller to observe.

To disable the scroll edge appearance for one or more edges, override contentScrollView(for:).

## See Also

### Working with scrolling content

func setContentScrollView(UIScrollView?)

Sets the scroll view that bars observe for all edges of the view.

func contentScrollView(for: NSDirectionalRectEdge) -> UIScrollView?

Returns the scroll view the view controller observes for the specified edge.

