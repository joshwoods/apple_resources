

- SwiftData
- ModelConfiguration
- ModelConfiguration.CloudKitDatabase
-  none 

Type Property

# none

Disables managed CloudKit sync.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+Swift 5.9+

``` source
static var none: ModelConfiguration.CloudKitDatabase { get }
```

## Mentioned in 

Syncing model data across a person’s devices

## See Also

### Getting discovery options

static var automatic: ModelConfiguration.CloudKitDatabase

Enables managed CloudKit sync using the primary ubiquity container from the app’s entitlements.

static func `private`(String) -> ModelConfiguration.CloudKitDatabase

Enables managed CloudKit sync using the specified ubiquity container.

