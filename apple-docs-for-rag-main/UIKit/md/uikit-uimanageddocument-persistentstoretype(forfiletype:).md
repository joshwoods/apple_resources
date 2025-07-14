

- UIKit
- UIManagedDocument
-  persistentStoreType(forFileType:) 

Instance Method

# persistentStoreType(forFileType:)

Returns the Core Data store type for a given document file type.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func persistentStoreType(forFileType fileType: String) -> String
```

## Parameters 

`fileType`  

The document file type.

## Return Value

The persistent store type for `fileType`.

## Discussion

Override this method to specify a persistent store type for a given document type.

The default returns NSSQLiteStoreType.

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

var modelConfiguration: String?

A model configuration name to be passed when configuring the persistent store.

