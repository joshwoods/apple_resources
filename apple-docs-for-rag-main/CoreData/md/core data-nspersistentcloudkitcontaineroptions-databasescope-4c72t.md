

- Core Data
- NSPersistentCloudKitContainerOptions
-  databaseScope 

Instance Property

# databaseScope

The database scope — public, private, or shared — to use for a specified store in a persistent CloudKit container.

CoreDataCloudKitiOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
var databaseScope: CKDatabase.Scope { get set }
```

## See Also

### Creating Container Options

init(containerIdentifier: String)

Initializes container options using the given CloudKit container identifier.

var containerIdentifier: String

The identifier of the CloudKit container associated with a given store description.

