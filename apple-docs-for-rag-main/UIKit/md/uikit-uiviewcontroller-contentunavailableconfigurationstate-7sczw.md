

- UIKit
- UIViewController
-  contentUnavailableConfigurationState 

Instance Property

# contentUnavailableConfigurationState

The current configuration state of the content-unavailable view.

iOS 17.0+iPadOS 17.0+Mac CatalysttvOS 17.0+visionOS

``` source
@MainActor @objc(_bridgedContentUnavailableConfigurationState) @preconcurrency
dynamic var contentUnavailableConfigurationState: UIContentUnavailableConfigurationState { get }
```

## Discussion

You can customize the configuration state by overriding this property in your subclass. Obtain the system instance from the superclass, and customize the state as appropriate.

## See Also

### Indicating missing content

var contentUnavailableConfiguration: (any UIContentConfiguration)?

The current content-unavailable configuration of the view controller.

func setNeedsUpdateContentUnavailableConfiguration()

Requests that the system update the content-unavailable configuration for the latest state.

func updateContentUnavailableConfiguration(using: UIContentUnavailableConfigurationState)

Updates the content-unavailable configuration for the provided state.

struct UIContentUnavailableConfiguration

A content configuration for a content-unavailable view.

