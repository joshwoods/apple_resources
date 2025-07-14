

- UIKit
- UIManagedDocument
-  persistentStoreOptions 

Instance Property

# persistentStoreOptions

Options used when creating the document’s persistent store.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var persistentStoreOptions: [AnyHashable : Any]? { get set }
```

## Discussion

By default, this value is `nil`.

To support automatic migration, you might pass a dictionary like that shown in the following example.

```
NSDictionary *options = @{
    NSMigratePersistentStoresAutomaticallyOption: @YES,
    NSInferMappingModelAutomaticallyOption: @YES
};
.persistentStoreOptions = options;
```

## See Also

### Managing the Core Data stack

func configurePersistentStoreCoordinator(for: URL, ofType: String, modelConfiguration: String?, storeOptions: [AnyHashable : Any]?) throws

Creates or loads the document’s persistent store.

var managedObjectContext: NSManagedObjectContext

The document’s managed object context.

var managedObjectModel: NSManagedObjectModel

The document’s managed object model.

var modelConfiguration: String?

A model configuration name to be passed when configuring the persistent store.

func persistentStoreType(forFileType: String) -> String

Returns the Core Data store type for a given document file type.

