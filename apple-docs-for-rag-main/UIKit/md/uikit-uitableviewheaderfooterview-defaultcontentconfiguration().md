

- UIKit
- UITableViewHeaderFooterView
-  defaultContentConfiguration() 

Instance Method

# defaultContentConfiguration()

Retrieves a default list content configuration for the view’s style.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
@MainActor @preconcurrency
func defaultContentConfiguration() -> UIListContentConfiguration
```

## Return Value

A default list content configuration. The system determines default values for the configuration according to the section where the view appears.

## Discussion

The default content configuration has preconfigured default styling, but doesn’t contain any content. After you get the default configuration, you assign your content to it, customize any other properties, and assign it to the view as the current contentConfiguration.

## See Also

### Managing the content

var contentConfiguration: (any UIContentConfiguration)?

The current content configuration of the view.

var automaticallyUpdatesContentConfiguration: Bool

A Boolean value that determines whether the view automatically updates its content configuration when its state changes.

var contentView: UIView

The content view of the header or footer.

