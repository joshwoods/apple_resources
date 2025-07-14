

- AppKit
- NSPersistentDocument
-  persistentStoreType(forFileType:) 

Instance Method

# persistentStoreType(forFileType:)

Returns the type of persistent store associated with the specified file type.

macOS

``` source
@MainActor
func persistentStoreType(forFileType fileType: String) -> String
```

## Parameters 

`fileType`  

A document file type.

## Return Value

The type of persistent store associated with `fileType`. For possible values, see NSPersistentStoreCoordinator.

## Discussion

You set the persistent store type in the application’s property list.

## See Also

### Managing the Persistence Objects

var managedObjectContext: NSManagedObjectContext?

The managed object context for the document.

var managedObjectModel: NSManagedObjectModel?

The managed object model of the document.

func configurePersistentStoreCoordinator(for: URL, ofType: String, modelConfiguration: String?, storeOptions: [String : Any]?) throws

Configures the receiver’s persistent store coordinator with the appropriate stores for a given URL.

