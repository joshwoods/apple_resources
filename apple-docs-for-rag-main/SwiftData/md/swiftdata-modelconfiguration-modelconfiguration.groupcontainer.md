

- SwiftData
- ModelConfiguration
-  ModelConfiguration.GroupContainer 

Structure

# ModelConfiguration.GroupContainer

A type that describes the options for detecting an app group container.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+Swift 5.9+

``` source
struct GroupContainer
```

## Topics

### Getting discovery options

static var automatic: ModelConfiguration.GroupContainer

Tells SwiftData to use the app’s primary group container as the root location for the persistent storage.

static func identifier(String) -> ModelConfiguration.GroupContainer

Tells SwiftData to use the specified group container as the root location for the app’s persistent storage.

static var none: ModelConfiguration.GroupContainer

Prevents SwiftData from using a group container as the root location for the app’s persistent storage.

## See Also

### Sharing and syncing the model store

let cloudKitContainerIdentifier: String?

The identifier of the configuration’s CloudKit database container.

let cloudKitDatabase: ModelConfiguration.CloudKitDatabase

The option to use when detecting the container of the preferred CloudKit database.

struct CloudKitDatabase

A type that describes the options for detecting a CloudKit database.

let groupAppContainerIdentifier: String?

The identifier of the configuration’s app group container.

let groupContainer: ModelConfiguration.GroupContainer

The option to use when detecting the preferred app group container.

