

- UIKit
- UIActivityItemsConfiguration
-  perItemMetadataProvider 

Instance Property

# perItemMetadataProvider

A closure that provides metadata for each activity item.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var perItemMetadataProvider: ((Int, UIActivityItemsConfigurationMetadataKey) -> Any?)? { get set }
```

## Mentioned in 

Collaborating and sharing copies of your data

## See Also

### Managing the configuration

var localObject: Any?

A local object that represents the configuration.

var metadataProvider: ((UIActivityItemsConfigurationMetadataKey) -> Any?)?

A closure that provides metadata for the activity items.

var applicationActivitiesProvider: (() -> [UIActivity])?

A closure that provides application acitivites for the activity items.

struct UIActivityItemsConfigurationMetadataKey

A structure that defines keys for the metadata associated with an activity items configuration.

