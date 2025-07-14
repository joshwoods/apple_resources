

- UIKit
- UIActivityItemsConfiguration
-  localObject 

Instance Property

# localObject

A local object that represents the configuration.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var localObject: Any? { get set }
```

## See Also

### Managing the configuration

var metadataProvider: ((UIActivityItemsConfigurationMetadataKey) -> Any?)?

A closure that provides metadata for the activity items.

var perItemMetadataProvider: ((Int, UIActivityItemsConfigurationMetadataKey) -> Any?)?

A closure that provides metadata for each activity item.

var applicationActivitiesProvider: (() -> [UIActivity])?

A closure that provides application acitivites for the activity items.

struct UIActivityItemsConfigurationMetadataKey

A structure that defines keys for the metadata associated with an activity items configuration.

