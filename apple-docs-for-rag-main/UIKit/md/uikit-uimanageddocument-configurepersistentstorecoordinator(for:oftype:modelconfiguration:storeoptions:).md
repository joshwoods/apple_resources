

- UIKit
- UIManagedDocument
-  configurePersistentStoreCoordinator(for:ofType:modelConfiguration:storeOptions:) 

Instance Method

# configurePersistentStoreCoordinator(for:ofType:modelConfiguration:storeOptions:)

Creates or loads the document’s persistent store.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func configurePersistentStoreCoordinator(
    for storeURL: URL,
    ofType fileType: String,
    modelConfiguration configuration: String?,
    storeOptions: [AnyHashable : Any]? = nil
) throws
```

## Parameters 

`storeURL`  

The URL for the persistent store.

`fileType`  

The document’s file type.

`configuration`  

The managed object model configuration to use.

`storeOptions`  

The options used to configure the persistent store coordinator.

## Discussion

You can override this method if you want customize the creation or loading of the document’s persistent store. For example, you can perform post-migration clean-up — if your app needs to migrate store data to use a new version of the managed object model, you can override this method to make additional modifications to the store after migration.

Handling Errors in Swift

In Swift, this method is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

When overriding this method, use the `throw` statement to throw an `NSError`, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Managing the Core Data stack

var managedObjectContext: NSManagedObjectContext

The document’s managed object context.

var managedObjectModel: NSManagedObjectModel

The document’s managed object model.

var persistentStoreOptions: [AnyHashable : Any]?

Options used when creating the document’s persistent store.

var modelConfiguration: String?

A model configuration name to be passed when configuring the persistent store.

func persistentStoreType(forFileType: String) -> String

Returns the Core Data store type for a given document file type.

