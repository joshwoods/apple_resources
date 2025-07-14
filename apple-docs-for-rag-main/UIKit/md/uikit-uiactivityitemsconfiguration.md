

- UIKit
-  UIActivityItemsConfiguration 

Class

# UIActivityItemsConfiguration

A configuration that allows a responder to export data through a variety of interactions.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class UIActivityItemsConfiguration
```

## Mentioned in 

Collaborating and sharing copies of your data

## Topics

### Creating an activity items configuration

init(objects: [any NSItemProviderWriting])

Initializes and returns an activity items configuration with the specified objects.

init(itemProviders: [NSItemProvider])

Initializes and returns an activity items configuration with the specified item providers.

### Managing the configuration

var localObject: Any?

A local object that represents the configuration.

var metadataProvider: ((UIActivityItemsConfigurationMetadataKey) -> Any?)?

A closure that provides metadata for the activity items.

var perItemMetadataProvider: ((Int, UIActivityItemsConfigurationMetadataKey) -> Any?)?

A closure that provides metadata for each activity item.

var applicationActivitiesProvider: (() -> [UIActivity])?

A closure that provides application acitivites for the activity items.

struct UIActivityItemsConfigurationMetadataKey

A structure that defines keys for the metadata associated with an activity items configuration.

### Managing supported interactions

var supportedInteractions: [UIActivityItemsConfigurationInteraction]

The types of interactions that the configuration supports.

struct UIActivityItemsConfigurationInteraction

A structure that describes types of interactions.

### Managing previews

var previewProvider: ((Int, UIActivityItemsConfigurationPreviewIntent, CGSize) -> NSItemProvider?)?

A closure that provides previews for the activity items.

struct UIActivityItemsConfigurationPreviewIntent

A structure that specifies the types of activity item previews.

### Restricting the sharing mode

class CollaborationModeRestriction

An object that disables the sharing mode and optionally displays an alert.

enum UIActivityCollaborationMode

A value that defines how the system shares an item.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable
- UIActivityItemsConfigurationReading

## See Also

### Initializing the activity view controller

init(activityItems: [Any], applicationActivities: [UIActivity]?)

Initializes a new activity view controller object that acts on the specified data.

convenience init(activityItemsConfiguration: any UIActivityItemsConfigurationReading)

Initializes a new activity view controller object that acts on the specified configuration.

protocol UIActivityItemsConfigurationReading

A set of methods adopted by an object so that the object can act as an activity items configuration.

