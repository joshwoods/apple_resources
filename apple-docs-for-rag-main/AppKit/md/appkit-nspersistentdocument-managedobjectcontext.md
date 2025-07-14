

- AppKit
- NSPersistentDocument
-  managedObjectContext 

Instance Property

# managedObjectContext

The managed object context for the document.

macOS

``` source
@MainActor
var managedObjectContext: NSManagedObjectContext? { get set }
```

## Discussion

If a managed object context for the document does not exist, one is created automatically. If you want to customize the creation of the persistence stack, reimplement this property in your custom subclass and use your implementation to create the appropriate objects.

## See Also

### Related Documentation

Core Data Programming Guide

Document-Based App Programming Guide for Mac

### Managing the Persistence Objects

var managedObjectModel: NSManagedObjectModel?

The managed object model of the document.

func configurePersistentStoreCoordinator(for: URL, ofType: String, modelConfiguration: String?, storeOptions: [String : Any]?) throws

Configures the receiver’s persistent store coordinator with the appropriate stores for a given URL.

func persistentStoreType(forFileType: String) -> String

Returns the type of persistent store associated with the specified file type.

