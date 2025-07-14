

- UIKit
- UIViewController
-  contentUnavailableConfiguration 

Instance Property

# contentUnavailableConfiguration

The current content-unavailable configuration of the view controller.

iOS 17.0+iPadOS 17.0+Mac CatalysttvOS 17.0+visionOS

``` source
@MainActor @preconcurrency
var contentUnavailableConfiguration: (any UIContentConfiguration)? { get set }
```

## Discussion

Use this property to configure a content-unavailable view that the view controller manages. The value of this property is commonly an instance of UIContentUnavailableConfiguration, but you can use other types of content configuration, including a UIHostingConfiguration, to display a SwiftUI view.

## See Also

### Indicating missing content

var contentUnavailableConfigurationState: UIContentUnavailableConfigurationState

The current configuration state of the content-unavailable view.

func setNeedsUpdateContentUnavailableConfiguration()

Requests that the system update the content-unavailable configuration for the latest state.

func updateContentUnavailableConfiguration(using: UIContentUnavailableConfigurationState)

Updates the content-unavailable configuration for the provided state.

struct UIContentUnavailableConfiguration

A content configuration for a content-unavailable view.

