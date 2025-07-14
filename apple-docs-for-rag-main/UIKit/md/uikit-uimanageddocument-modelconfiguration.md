

- UIKit
- UIManagedDocument
-  modelConfiguration 

Instance Property

# modelConfiguration

A model configuration name to be passed when configuring the persistent store.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var modelConfiguration: String? { get set }
```

## Discussion

By default, this value is `nil`.

## See Also

### Managing the Core Data stack

func configurePersistentStoreCoordinator(for: URL, ofType: String, modelConfiguration: String?, storeOptions: [AnyHashable : Any]?) throws

Creates or loads the document’s persistent store.

var managedObjectContext: NSManagedObjectContext

The document’s managed object context.

var managedObjectModel: NSManagedObjectModel

The document’s managed object model.

var persistentStoreOptions: [AnyHashable : Any]?

Options used when creating the document’s persistent store.

func persistentStoreType(forFileType: String) -> String

Returns the Core Data store type for a given document file type.

