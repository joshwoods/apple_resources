

- UIKit
- UIManagedDocument
-  managedObjectContext 

Instance Property

# managedObjectContext

The document’s managed object context.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var managedObjectContext: NSManagedObjectContext { get }
```

## Discussion

The document automatically creates a managed object context using its persistent store coordinator.

### Special considerations

You must not use the document’s managed object context in writeAdditionalContent(_:to:originalContentsURL:), or any of the asynchronous UIDocument methods.

## See Also

### Managing the Core Data stack

func configurePersistentStoreCoordinator(for: URL, ofType: String, modelConfiguration: String?, storeOptions: [AnyHashable : Any]?) throws

Creates or loads the document’s persistent store.

var managedObjectModel: NSManagedObjectModel

The document’s managed object model.

var persistentStoreOptions: [AnyHashable : Any]?

Options used when creating the document’s persistent store.

var modelConfiguration: String?

A model configuration name to be passed when configuring the persistent store.

func persistentStoreType(forFileType: String) -> String

Returns the Core Data store type for a given document file type.

