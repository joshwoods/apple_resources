

- Core Data
- NSIncrementalStore
-  execute(\_:with:) 

Instance Method

# execute(\_:with:)

Returns a value as appropriate for the given request, or nil if the request cannot be completed.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func execute(
    _ request: NSPersistentStoreRequest,
    with context: NSManagedObjectContext?
) throws -> Any
```

## Parameters 

`request`  

A fetch request.

`context`  

The managed object context used to execute `request`.

## Return Value

A value as appropriate for `request`, or `nil` if the request cannot be completed

## Discussion

The value to return depends on the result type (see resultType) of `request`:

- If it is `NSManagedObjectResultType`, `NSManagedObjectIDResultType`, or `NSDictionaryResultType`, the method should return an array containing all objects in the store matching the request.

- If it is `NSCountResultType`, the method should return an array containing an `NSNumber` whose value is the count of all objects in the store matching the request.

- If the request is a save request, the method should return an empty array.

If the save request contains nil values for the inserted/updated/deleted/locked collections; you should treat it as a request to save the store metadata.

You should implement this method conservatively, and expect that unknown request types may at some point be passed to the method. The correct behavior in these cases is to return `nil` and an error.

## See Also

### Manipulating Managed Objects

func newValuesForObject(with: NSManagedObjectID, with: NSManagedObjectContext) throws -> NSIncrementalStoreNode

Returns an incremental store node encapsulating the persistent external values of the object with a given object ID.

func newValue(forRelationship: NSRelationshipDescription, forObjectWith: NSManagedObjectID, with: NSManagedObjectContext?) throws -> Any

Returns the relationship for the given relationship of the object with a given object ID.

func obtainPermanentIDs(for: [NSManagedObject]) throws -> [NSManagedObjectID]

Returns an array containing the object IDs for a given array of newly-inserted objects.

func newObjectID(for: NSEntityDescription, referenceObject: Any) -> NSManagedObjectID

Returns a new object ID that uses given data as the key.

func referenceObject(for: NSManagedObjectID) -> Any

Returns the reference data used to construct a given object ID.

