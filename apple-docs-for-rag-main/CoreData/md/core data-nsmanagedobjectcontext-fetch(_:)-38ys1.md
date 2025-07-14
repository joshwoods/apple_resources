

- Core Data
- NSManagedObjectContext
-  fetch(\_:) 

Instance Method

# fetch(\_:)

Returns an array of objects that meet the criteria of the specified fetch request.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
func fetch(_ request: NSFetchRequest) throws -> [Any]
```

## Parameters 

`request`  

A fetch request that specifies the search criteria for the fetch.

## Return Value

An array of objects that meet the criteria specified by `request` fetched from the receiver and from the persistent stores associated with the receiver’s persistent store coordinator. If an error occurs, returns `nil`. If no objects match the criteria specified by `request`, returns an empty array.

## Discussion

Returned objects are registered with the receiver.

The following points are important to consider:

- If the fetch request has no predicate, then all instances of the specified entity are retrieved, modulo other criteria below.

- An object that meets the criteria specified by `request` (it is an instance of the entity specified by the request, and it matches the request’s predicate if there is one) and that has been inserted into a context but which is not yet saved to a persistent store, is retrieved if the fetch request is executed on that context.

- If an object in a context has been modified, a predicate is evaluated against its modified state, not against the current state in the persistent store. Therefore, if an object in a context has been modified such that it meets the fetch request’s criteria, the request retrieves it even if changes have not been saved to the store and the values in the store are such that it does not meet the criteria. Conversely, if an object in a context has been modified such that it does not match the fetch request, the fetch request will not retrieve it even if the version in the store does match.

- If an object has been deleted from the context, the fetch request does not retrieve it even if that deletion has not been saved to a store.

Objects that have been realized (populated, faults fired, “read from”, and so on) as well as pending updated, inserted, or deleted, are never changed by a fetch operation without developer intervention. If you fetch some objects, work with them, and then execute a new fetch that includes a superset of those objects, you do not get new instances or update data for the existing objects—you get the existing objects with their current in-memory state.

## See Also

### Related Documentation

Core Data Programming Guide

Predicate Programming Guide

Core Data Snippets

### Registering and fetching objects

func fetch&lt;T>(NSFetchRequest&lt;T>) throws -> [T]

Returns an array of items of the specified type that meet the fetch request’s critieria.

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

