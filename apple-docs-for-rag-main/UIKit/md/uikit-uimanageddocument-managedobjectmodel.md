

- UIKit
- UIManagedDocument
-  managedObjectModel 

Instance Property

# managedObjectModel

The document’s managed object model.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var managedObjectModel: NSManagedObjectModel { get }
```

## Discussion

Persistent documents always have a managed object model. The default model is the union of all models in the main bundle. You can specify a configuration to use with modelConfiguration. You can subclass UIManagedDocument to override this method if you need custom behavior.

## See Also

### Managing the Core Data stack

func configurePersistentStoreCoordinator(for: URL, ofType: String, modelConfiguration: String?, storeOptions: [AnyHashable : Any]?) throws

Creates or loads the document’s persistent store.

var managedObjectContext: NSManagedObjectContext

The document’s managed object context.

var persistentStoreOptions: [AnyHashable : Any]?

Options used when creating the document’s persistent store.

var modelConfiguration: String?

A model configuration name to be passed when configuring the persistent store.

func persistentStoreType(forFileType: String) -> String

Returns the Core Data store type for a given document file type.

