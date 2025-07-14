

- UIKit
- UIViewController
-  viewDidLayoutSubviews() 

Instance Method

# viewDidLayoutSubviews()

Notifies the view controller when its view finishes laying out its subviews.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func viewDidLayoutSubviews()
```

## Mentioned in 

Displaying and managing views with a view controller

## Discussion

When the bounds change for a view controller’s view, the view adjusts the positions of its subviews and then the system calls this method. However, this method being called *does not* indicate that the individual layouts of the view’s subviews have been adjusted. Each subview is responsible for adjusting its own layout.

Your view controller can override this method to make changes after the view lays out its subviews. The default implementation of this method does nothing.

In iOS 18 and later, UIKit supports automatic trait tracking inside this method for traits from this view controller’s `traitCollection` and the `traitCollection` of its view. For more information, see Automatic trait tracking.

## See Also

### View controllers

func viewWillLayoutSubviews()

Notifies the view controller that its view is about to lay out its subviews.

func updateViewConstraints()

Notifies the view controller when its view needs to update its constraints.

func updateContentUnavailableConfiguration(using: UIContentUnavailableConfigurationState)

Updates the content-unavailable configuration for the provided state.

