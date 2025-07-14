

- SwiftData
- ModelConfiguration
-  ModelConfiguration.CloudKitDatabase 

Structure

# ModelConfiguration.CloudKitDatabase

A type that describes the options for detecting a CloudKit database.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+Swift 5.9+

``` source
struct CloudKitDatabase
```

## Topics

### Getting discovery options

static var automatic: ModelConfiguration.CloudKitDatabase

Enables managed CloudKit sync using the primary ubiquity container from the app’s entitlements.

static func `private`(String) -> ModelConfiguration.CloudKitDatabase

Enables managed CloudKit sync using the specified ubiquity container.

static var none: ModelConfiguration.CloudKitDatabase

Disables managed CloudKit sync.

## See Also

### Sharing and syncing the model store

let cloudKitContainerIdentifier: String?

The identifier of the configuration’s CloudKit database container.

let cloudKitDatabase: ModelConfiguration.CloudKitDatabase

The option to use when detecting the container of the preferred CloudKit database.

let groupAppContainerIdentifier: String?

The identifier of the configuration’s app group container.

let groupContainer: ModelConfiguration.GroupContainer

The option to use when detecting the preferred app group container.

struct GroupContainer

A type that describes the options for detecting an app group container.

