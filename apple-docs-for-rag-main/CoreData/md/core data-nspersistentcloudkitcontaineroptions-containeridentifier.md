

- Core Data
- NSPersistentCloudKitContainerOptions
-  containerIdentifier 

Instance Property

# containerIdentifier

The identifier of the CloudKit container associated with a given store description.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var containerIdentifier: String { get }
```

## See Also

### Creating Container Options

init(containerIdentifier: String)

Initializes container options using the given CloudKit container identifier.

var databaseScope: CKDatabase.Scope

The database scope — public, private, or shared — to use for a specified store in a persistent CloudKit container.

