

- UIKit
- UIContentUnavailableConfiguration
-  empty() 

Type Method

# empty()

Creates the default configuration for unavailable content.

iOS 17.0+iPadOS 17.0+Mac CatalysttvOS 17.0+visionOS

``` source
static func empty() -> UIContentUnavailableConfiguration
```

## Return Value

A new configuration.

## Discussion

Use this method to create a new configuration to customize. This is useful if your empty content doesn’t fit the uses covered by configurations available with search() or loading().

