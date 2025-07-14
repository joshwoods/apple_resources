

- AppKit
- NSPersistentDocument
-  configurePersistentStoreCoordinator(for:ofType:modelConfiguration:storeOptions:) 

Instance Method

# configurePersistentStoreCoordinator(for:ofType:modelConfiguration:storeOptions:)

Configures the receiver’s persistent store coordinator with the appropriate stores for a given URL.

macOS 10.5+

``` source
@MainActor
func configurePersistentStoreCoordinator(
    for url: URL,
    ofType fileType: String,
    modelConfiguration configuration: String?,
    storeOptions: [String : Any]? = nil
) throws
```

## Parameters 

`url`  

An URL that specifies the location of the document’s store.

`fileType`  

The document type.

`configuration`  

The name of the managed object model configuration to use. (The managed object model is associated with the persistent store coordinator.) Pass `nil` if you do not want to specify a configuration.

`storeOptions`  

Options for the store. See “Store Options” in NSPersistentStoreCoordinator for possible values.

## Discussion

This method is invoked automatically when an existing document is opened. You override this method to customize creation of a persistent store for a given document or store type. You can retrieve the persistent store coordinator with the following code:

```
[[self managedObjectContext] persistentStoreCoordinator];
```

You can override this method to create the store to save to or load from (invoked from within the other `NSDocument` methods to read/write files), which gives developers the ability to load/save from/to different persistent store types (default type is XML).

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Managing the Persistence Objects

var managedObjectContext: NSManagedObjectContext?

The managed object context for the document.

var managedObjectModel: NSManagedObjectModel?

The managed object model of the document.

func persistentStoreType(forFileType: String) -> String

Returns the type of persistent store associated with the specified file type.

