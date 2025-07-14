

- UIKit
- UIPresentationController
-  frameOfPresentedViewInContainerView 

Instance Property

# frameOfPresentedViewInContainerView

The frame rectangle to assign to the presented view at the end of the animations.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var frameOfPresentedViewInContainerView: CGRect { get }
```

## Return Value

The rectangle of the presented view controller’s view, specified in the container view’s coordinate system.

## Discussion

The default implementation of this method returns the frame rectangle of the container view, which results in the presented view controller’s content occupying the entire presentation space. You can override this method and return a different frame rectangle as needed. For example, you might specify a smaller frame rectangle if you want some of the underlying content to show around the edges of the presented view.

UIKit calls this method multiple times during the course of a presentation, so your implementation should return the same frame rectangle each time. Do not use this method to make changes to your view hierarchy or perform other one-time tasks.

## See Also

### Adjusting the size and layout of the presentation

func containerViewWillLayoutSubviews()

Notifies the presentation controller that layout is about to begin on the views of the container view.

func containerViewDidLayoutSubviews()

Notifies the presentation controller when layout ends on the views of the container view.

