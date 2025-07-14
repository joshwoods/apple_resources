

- Core Data
- NSPersistentContainer
-  persistentStoreDescriptions 

Instance Property

# persistentStoreDescriptions

The descriptions of the container’s persistent stores.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var persistentStoreDescriptions: [NSPersistentStoreDescription] { get set }
```

## Discussion

If you want to override the type (or types) of persistent store(s) used by the persistent container, you can set this property with an array of NSPersistentStoreDescription objects.

If you will be configuring custom persistent store descriptions, you must set this property before calling loadPersistentStores(completionHandler:).

## See Also

### Managing Persistent Stores

func loadPersistentStores(completionHandler: (NSPersistentStoreDescription, (any Error)?) -> Void)

Loads the persistent stores.

