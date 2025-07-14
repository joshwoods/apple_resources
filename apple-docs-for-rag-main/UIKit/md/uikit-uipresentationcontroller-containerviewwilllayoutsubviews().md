

- UIKit
- UIPresentationController
-  containerViewWillLayoutSubviews() 

Instance Method

# containerViewWillLayoutSubviews()

Notifies the presentation controller that layout is about to begin on the views of the container view.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func containerViewWillLayoutSubviews()
```

## Discussion

UIKit calls this method before adjusting the layout of the views in the container view. Use this method and the containerViewDidLayoutSubviews() method to update any custom views managed by your presentation controller.

In iOS 18 and later, UIKit supports automatic trait tracking inside this method for traits from this presentation controller’s `traitCollection` and the `traitCollection` of its containerView. For more information, see Automatic trait tracking.

## See Also

### Presentation controllers

func containerViewDidLayoutSubviews()

Notifies the presentation controller when layout ends on the views of the container view.

