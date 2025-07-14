

- UIKit
- UIViewController
-  updateContentUnavailableConfiguration(using:) 

Instance Method

# updateContentUnavailableConfiguration(using:)

Updates the content-unavailable configuration for the provided state.

iOS 17.0+iPadOS 17.0+Mac CatalysttvOS 17.0+visionOS

``` source
@MainActor @objc(_bridgedUpdateContentUnavailableConfigurationUsingState:) @preconcurrency
dynamic func updateContentUnavailableConfiguration(using state: UIContentUnavailableConfigurationState)
```

## Parameters 

`state`  

The current configuration state for a content-unavailable view.

## Discussion

Override this method to update the value of contentUnavailableConfiguration as appropriate for the given state.

Don’t call this method directly. Instead, call setNeedsUpdateContentUnavailableConfiguration() to tell the system to request an update.

In iOS 18 and later, UIKit supports automatic trait tracking inside this method for traits from this view controller’s `traitCollection` and the `traitCollection` of its view. For more information, see Automatic trait tracking.

## See Also

### View controllers

func viewWillLayoutSubviews()

Notifies the view controller that its view is about to lay out its subviews.

func viewDidLayoutSubviews()

Notifies the view controller when its view finishes laying out its subviews.

func updateViewConstraints()

Notifies the view controller when its view needs to update its constraints.

