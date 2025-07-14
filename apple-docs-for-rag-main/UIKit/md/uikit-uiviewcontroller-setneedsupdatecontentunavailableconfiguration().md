

- UIKit
- UIViewController
-  setNeedsUpdateContentUnavailableConfiguration() 

Instance Method

# setNeedsUpdateContentUnavailableConfiguration()

Requests that the system update the content-unavailable configuration for the latest state.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+tvOS 17.0+visionOS 1.0+

``` source
@MainActor
func setNeedsUpdateContentUnavailableConfiguration()
```

## See Also

### Indicating missing content

var contentUnavailableConfiguration: (any UIContentConfiguration)?

The current content-unavailable configuration of the view controller.

var contentUnavailableConfigurationState: UIContentUnavailableConfigurationState

The current configuration state of the content-unavailable view.

func updateContentUnavailableConfiguration(using: UIContentUnavailableConfigurationState)

Updates the content-unavailable configuration for the provided state.

struct UIContentUnavailableConfiguration

A content configuration for a content-unavailable view.

