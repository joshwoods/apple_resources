

- UIKit
- UIActivityItemsConfiguration
-  applicationActivitiesProvider 

Instance Property

# applicationActivitiesProvider

A closure that provides application acitivites for the activity items.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var applicationActivitiesProvider: (() -> [UIActivity])? { get set }
```

## See Also

### Managing the configuration

var localObject: Any?

A local object that represents the configuration.

var metadataProvider: ((UIActivityItemsConfigurationMetadataKey) -> Any?)?

A closure that provides metadata for the activity items.

var perItemMetadataProvider: ((Int, UIActivityItemsConfigurationMetadataKey) -> Any?)?

A closure that provides metadata for each activity item.

struct UIActivityItemsConfigurationMetadataKey

A structure that defines keys for the metadata associated with an activity items configuration.

