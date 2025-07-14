

- UIKit
- UIActivityItemsConfiguration
-  metadataProvider 

Instance Property

# metadataProvider

A closure that provides metadata for the activity items.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var metadataProvider: ((UIActivityItemsConfigurationMetadataKey) -> Any?)? { get set }
```

## See Also

### Managing the configuration

var localObject: Any?

A local object that represents the configuration.

var perItemMetadataProvider: ((Int, UIActivityItemsConfigurationMetadataKey) -> Any?)?

A closure that provides metadata for each activity item.

var applicationActivitiesProvider: (() -> [UIActivity])?

A closure that provides application acitivites for the activity items.

struct UIActivityItemsConfigurationMetadataKey

A structure that defines keys for the metadata associated with an activity items configuration.

