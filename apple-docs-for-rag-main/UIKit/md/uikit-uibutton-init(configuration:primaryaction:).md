

- UIKit
- UIButton
-  init(configuration:primaryAction:) 

Initializer

# init(configuration:primaryAction:)

Creates a new button with the specified configuration and registers the primary action event.

iOS 15.0+iPadOS 15.0+Mac CatalysttvOS 15.0+visionOS

``` source
@MainActor @preconcurrency
convenience init(
    configuration: UIButton.Configuration,
    primaryAction: UIAction? = nil
)
```

## Parameters 

`configuration`  

The button configuration.

`primaryAction`  

The action to perform for the primaryActionTriggered control event.

## Discussion

If the primary action contains a title or an image, this method copies them to the configuration and the button displays them.

## See Also

### Creating buttons from a configuration object

struct Configuration

A configuration that specifies the appearance and behavior of a button and its contents.

