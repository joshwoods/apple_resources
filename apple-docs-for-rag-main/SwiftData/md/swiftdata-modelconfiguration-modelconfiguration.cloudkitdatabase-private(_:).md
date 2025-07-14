

- SwiftData
- ModelConfiguration
- ModelConfiguration.CloudKitDatabase
-  private(\_:) 

Type Method

# private(\_:)

Enables managed CloudKit sync using the specified ubiquity container.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+Swift 5.9+

``` source
static func `private`(_ privateDBName: String) -> ModelConfiguration.CloudKitDatabase
```

## Parameters 

`privateDBName`  

The identifier of the iCloud ubiquity container to use. You find these in the iCloud capabilities section of your Xcode project. For more information, see Configuring iCloud services.

## See Also

### Getting discovery options

static var automatic: ModelConfiguration.CloudKitDatabase

Enables managed CloudKit sync using the primary ubiquity container from the app’s entitlements.

static var none: ModelConfiguration.CloudKitDatabase

Disables managed CloudKit sync.

