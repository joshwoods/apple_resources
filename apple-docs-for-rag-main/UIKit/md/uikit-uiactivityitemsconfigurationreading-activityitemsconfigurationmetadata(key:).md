

- UIKit
- UIActivityItemsConfigurationReading
-  activityItemsConfigurationMetadata(key:) 

Instance Method

# activityItemsConfigurationMetadata(key:)

Returns the configuration for the specified metadata key.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func activityItemsConfigurationMetadata(key: UIActivityItemsConfigurationMetadataKey) -> Any?
```

## See Also

### Managing the Configuration

var itemProvidersForActivityItemsConfiguration: [NSItemProvider]

The item providers for the configuration.

**Required**

var applicationActivitiesForActivityItemsConfiguration: [UIActivity]?

The application activities, if any, for the configuration.

func activityItemsConfigurationMetadataForItem(at: Int, key: UIActivityItemsConfigurationMetadataKey) -> Any?

Returns the configuration for a particular item for the specified metadata key.

struct UIActivityItemsConfigurationMetadataKey

A structure that defines keys for the metadata associated with an activity items configuration.

