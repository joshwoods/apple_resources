

- SwiftData
- ModelConfiguration
- ModelConfiguration.CloudKitDatabase
-  automatic 

Type Property

# automatic

Enables managed CloudKit sync using the primary ubiquity container from the app’s entitlements.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+Swift 5.9+

``` source
static var automatic: ModelConfiguration.CloudKitDatabase { get }
```

## See Also

### Getting discovery options

static func `private`(String) -> ModelConfiguration.CloudKitDatabase

Enables managed CloudKit sync using the specified ubiquity container.

static var none: ModelConfiguration.CloudKitDatabase

Disables managed CloudKit sync.

