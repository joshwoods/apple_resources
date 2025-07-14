

- UIKit
-  UIActivityItemsConfigurationMetadataKey 

Structure

# UIActivityItemsConfigurationMetadataKey

A structure that defines keys for the metadata associated with an activity items configuration.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
struct UIActivityItemsConfigurationMetadataKey
```

## Topics

### Constants

static let title: UIActivityItemsConfigurationMetadataKey

A key for the title.

static let messageBody: UIActivityItemsConfigurationMetadataKey

A key for the message body.

static let linkPresentationMetadata: UIActivityItemsConfigurationMetadataKey

static let shareRecipients: UIActivityItemsConfigurationMetadataKey

static let collaborationModeRestrictions: UIActivityItemsConfigurationMetadataKey

### Initializers

init(String)

Creates an activity items configuration metadata key.

init(rawValue: String)

Creates an activity items configuration metadata key with the specified raw value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Managing the configuration

var localObject: Any?

A local object that represents the configuration.

var metadataProvider: ((UIActivityItemsConfigurationMetadataKey) -> Any?)?

A closure that provides metadata for the activity items.

var perItemMetadataProvider: ((Int, UIActivityItemsConfigurationMetadataKey) -> Any?)?

A closure that provides metadata for each activity item.

var applicationActivitiesProvider: (() -> [UIActivity])?

A closure that provides application acitivites for the activity items.

