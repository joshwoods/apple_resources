

- Core Data
- NSPersistentCloudKitContainerOptions
-  init(containerIdentifier:) 

Initializer

# init(containerIdentifier:)

Initializes container options using the given CloudKit container identifier.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(containerIdentifier: String)
```

## See Also

### Creating Container Options

var containerIdentifier: String

The identifier of the CloudKit container associated with a given store description.

var databaseScope: CKDatabase.Scope

The database scope — public, private, or shared — to use for a specified store in a persistent CloudKit container.

