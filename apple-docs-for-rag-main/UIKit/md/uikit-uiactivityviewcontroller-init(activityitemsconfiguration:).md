

- UIKit
- UIActivityViewController
-  init(activityItemsConfiguration:) 

Initializer

# init(activityItemsConfiguration:)

Initializes a new activity view controller object that acts on the specified configuration.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
@MainActor
convenience init(activityItemsConfiguration: any UIActivityItemsConfigurationReading)
```

## See Also

### Initializing the activity view controller

init(activityItems: [Any], applicationActivities: [UIActivity]?)

Initializes a new activity view controller object that acts on the specified data.

class UIActivityItemsConfiguration

A configuration that allows a responder to export data through a variety of interactions.

protocol UIActivityItemsConfigurationReading

A set of methods adopted by an object so that the object can act as an activity items configuration.

