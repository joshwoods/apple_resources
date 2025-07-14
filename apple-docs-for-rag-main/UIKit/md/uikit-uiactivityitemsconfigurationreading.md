

- UIKit
-  UIActivityItemsConfigurationReading 

Protocol

# UIActivityItemsConfigurationReading

A set of methods adopted by an object so that the object can act as an activity items configuration.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
protocol UIActivityItemsConfigurationReading : NSObjectProtocol
```

## Topics

### Managing the Configuration

var itemProvidersForActivityItemsConfiguration: [NSItemProvider]

The item providers for the configuration.

**Required**

var applicationActivitiesForActivityItemsConfiguration: [UIActivity]?

The application activities, if any, for the configuration.

func activityItemsConfigurationMetadata(key: UIActivityItemsConfigurationMetadataKey) -> Any?

Returns the configuration for the specified metadata key.

func activityItemsConfigurationMetadataForItem(at: Int, key: UIActivityItemsConfigurationMetadataKey) -> Any?

Returns the configuration for a particular item for the specified metadata key.

struct UIActivityItemsConfigurationMetadataKey

A structure that defines keys for the metadata associated with an activity items configuration.

### Managing Supported Interactions

func activityItemsConfigurationSupports(interaction: UIActivityItemsConfigurationInteraction) -> Bool

Returns a Boolean value that indicates whether the activity items configuration supports the specified type of interaction.

struct UIActivityItemsConfigurationInteraction

A structure that describes types of interactions.

### Managing Previews

func activityItemsConfigurationPreviewForItem(at: Int, intent: UIActivityItemsConfigurationPreviewIntent, suggestedSize: CGSize) -> NSItemProvider?

Returns an activity items configuration preview for the specified item and preview size.

struct UIActivityItemsConfigurationPreviewIntent

A structure that specifies the types of activity item previews.

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- UIActivityItemsConfiguration

## See Also

### Initializing the activity view controller

init(activityItems: [Any], applicationActivities: [UIActivity]?)

Initializes a new activity view controller object that acts on the specified data.

convenience init(activityItemsConfiguration: any UIActivityItemsConfigurationReading)

Initializes a new activity view controller object that acts on the specified configuration.

class UIActivityItemsConfiguration

A configuration that allows a responder to export data through a variety of interactions.

