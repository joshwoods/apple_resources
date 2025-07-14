

- UIKit
- UIViewController
-  setContentScrollView(\_:) 

Instance Method

# setContentScrollView(\_:)

Sets the scroll view that bars observe for all edges of the view.

iOS 15.0+iPadOS 15.0+Mac CatalysttvOS 15.0+visionOS

``` source
@MainActor @preconcurrency
func setContentScrollView(_ scrollView: UIScrollView?)
```

## Parameters 

`scrollView`  

The scroll view to observe.

## Discussion

Calling this convenience method is identical to calling setContentScrollView(_:for:) and passing all for the `edge` parameter.

## See Also

### Working with scrolling content

func setContentScrollView(UIScrollView?, for: NSDirectionalRectEdge)

Sets the scroll view that bars observe for the specified edge.

func contentScrollView(for: NSDirectionalRectEdge) -> UIScrollView?

Returns the scroll view the view controller observes for the specified edge.

