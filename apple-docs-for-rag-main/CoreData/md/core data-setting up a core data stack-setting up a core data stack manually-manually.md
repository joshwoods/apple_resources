

- Core Data
- Setting up a Core Data stack
-  Setting up a Core Data stack manually 

Article

# Setting up a Core Data stack manually

Create the individual components that Core Data requires manually, to support earlier versions of Apple operating systems.

## Overview

If your app targets iOS 10+, macOS 10.12+, tvOS 10+, watchOS 3+, or visionOS 1+, you can use NSPersistentContainer to simplify creation and management of the Core Data stack. Otherwise, you need to manually create an NSManagedObjectModel, NSPersistentStoreCoordinator, and at least one NSManagedObjectContext.

### Create a managed object model

To instantiate an NSManagedObjectModel, pass in a URL that points to the compiled version of the `.xcdatamodeld` file. This `.momd` file is typically part of your app bundle.

```
// Get a URL to the compiled model in the app bundle.
guard let modelURL = Bundle.main.url(forResource: "DataModel",
                                     withExtension: "momd") else {
    fatalError("Failed to find data model")
}

// Use the URL to create a managed object model.
guard let model = NSManagedObjectModel(contentsOf: modelURL) else {
    fatalError("Failed to create model from file: \(modelURL)")
}
```

### Create a persistent store coordinator

Next, pass the managed object model to the NSPersistentStoreCoordinator initializer to create a store coordinator with that model.

```
// Use the managed object model to create a persistent store coordinator.
let coordinator = NSPersistentStoreCoordinator(managedObjectModel: managedObjectModel)
```

#### Add a persistent store to the coordinator

If you want Core Data to persist your data model to disk, tell the store coordinator where the file exists and what format to use.

```
// Get the URL to the Document directory.
let documentDirectoryURL = FileManager.default.urls(for: .documentDirectory,
                                                    in: .userDomainMask).last
// Create a URL to the data store.
guard let storeURL = URL(string: "DataModel.sqlite",
                         relativeTo: documentDirectoryURL) else {
    fatalError("Failed to create store URL")
}

do {
    // Set the options to enable lightweight data migrations.
    let options = [NSMigratePersistentStoresAutomaticallyOption: true,
                         NSInferMappingModelAutomaticallyOption: true]
    // Add the store to the coordinator.
    _ = try coordinator.addPersistentStore(type: .sqlite, at: storeURL,
                                       options: options)
} catch {
    fatalError("Failed to add persistent store: \(error.localizedDescription)")
}
```

Important

If you don’t use NSPersistentContainer to set up your Core Data stack, you also need to manually set the options to enable lightweight data migrations. For more information, see Migrating your data model automatically.

There are advantages and disadvantages to each of the store types. Refer to the NSPersistentStoreCoordinator documentation for details on each store type.

### Create a managed object context

Create an NSManagedObjectContext, and set its store coordinator property.

```
// Create a context to interact with managed objects.
let context = NSManagedObjectContext(concurrencyType: .mainQueueConcurrencyType)
// Assign the coordinator to the context.
context.persistentStoreCoordinator = persistentStoreCoordinator
```

Your app uses this context to interact with Core Data. Pass a reference to this context to your user interface. For additional information, see Inject the managed object context.

