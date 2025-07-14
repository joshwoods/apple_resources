

- Core Data
- NSManagedObjectContext
-  fetch(\_:) 

Instance Method

# fetch(\_:)

Returns an array of items of the specified type that meet the fetch request’s critieria.

iOS 3.0+iPadOS 3.0+Mac CatalystmacOS 10.4+tvOS 3.0+visionOSwatchOS 1.0+

``` source
func fetch(_ request: NSFetchRequest) throws -> [T] where T : NSFetchRequestResult
```

## Parameters 

`request`  

The fetch request that specifies the search criteria.

## Mentioned in 

Accessing data when the store changes

## Discussion

This method fetches objects from the context and the persistent stores that you associate with the context’s persistent store coordinator. The method registers any objects it retrieves from a store with the context.

Consider the following when fetching:

- If the fetch request doesn’t have a predicate, it returns all instances of the specified entity.

- The fetch results include any object in the context that’s an instance of the request’s entity, and that meets the request’s criteria, even if the context has yet to save the object to a persistent store.

- The fetch request evalutes the in-memory state of each object. Therefore, the fetch results include any unsaved objects with changes that cause them to meet the request’s criteria, even if their counterparts in the persistent store don’t. Conversely, the results don’t include unsaved objects with in-memory changes that mean they no longer meet the criteria, even if their store versions do.

- The fetch results don’t include deleted objects, even if the context has yet to save the deletion to the persistent store.

A fetch never changes realized objects, or those with pending changes, without developer intervention. If you fetch objects, modify them, and then execute a new fetch that includes a superset of those objects, you don’t receive new instances of those objects. Instead, you receive the existing objects with their current in-memory state.

## See Also

### Registering and fetching objects

func fetch(NSFetchRequest&lt;any NSFetchRequestResult>) throws -> [Any]

Returns an array of objects that meet the criteria of the specified fetch request.

func count(for: NSFetchRequest&lt;any NSFetchRequestResult>) throws -> Int

Returns the number of objects the specified request fetches when it executes.

func registeredObject(for: NSManagedObjectID) -> NSManagedObject?

Returns an object that exists in the context.

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

