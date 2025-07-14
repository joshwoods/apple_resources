

- Core Data
- NSManagedObjectContext
-  registeredObject(for:) 

Instance Method

# registeredObject(for:)

Returns an object that exists in the context.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func registeredObject(for objectID: NSManagedObjectID) -> NSManagedObject?
```

## Parameters 

`objectID`  

The identifier of the object to retrieve. For more information, see NSManagedObjectID.

## Return Value

The identified object, if it’s known to the context; otherwise, `nil`.

## Discussion

This method provides a convenient way to retrieve an object from the context’s registeredObjects property. A `nil` return value means the context doesn’t recognize the specified object; the object might still exist in the persistent store. If you need to query both the context and the store, use existingObject(with:) instead.

## See Also

### Registering and fetching objects

func fetch(NSFetchRequest&lt;any NSFetchRequestResult>) throws -> [Any]

Returns an array of objects that meet the criteria of the specified fetch request.

func fetch&lt;T>(NSFetchRequest&lt;T>) throws -> [T]

Returns an array of items of the specified type that meet the fetch request’s critieria.

func count(for: NSFetchRequest&lt;any NSFetchRequestResult>) throws -> Int

Returns the number of objects the specified request fetches when it executes.

func object(with: NSManagedObjectID) -> NSManagedObject

Returns either an existing object from the context or a fault that represents that object.

func existingObject(with: NSManagedObjectID) throws -> NSManagedObject

Returns an existing object from either the context or the persistent store.

var registeredObjects: Set&lt;NSManagedObject>

The set of registered managed objects in the context.

func count&lt;T>(for: NSFetchRequest&lt;T>) throws -> Int

Returns a count of the objects the specified request fetches when it executes.

func execute(NSPersistentStoreRequest) throws -> NSPersistentStoreResult

Passes a request to the persistent store without affecting the contents of the managed object context, and returns a persistent store result.

func refreshAllObjects()

Refreshes all of the registered managed objects in the context.

var retainsRegisteredObjects: Bool

A Boolean value that indicates whether the context keeps strong references to all registered managed objects.

