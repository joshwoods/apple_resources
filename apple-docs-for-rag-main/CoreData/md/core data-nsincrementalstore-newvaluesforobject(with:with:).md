

- Core Data
- NSIncrementalStore
-  newValuesForObject(with:with:) 

Instance Method

# newValuesForObject(with:with:)

Returns an incremental store node encapsulating the persistent external values of the object with a given object ID.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func newValuesForObject(
    with objectID: NSManagedObjectID,
    with context: NSManagedObjectContext
) throws -> NSIncrementalStoreNode
```

## Parameters 

`objectID`  

The ID of the object for which values are requested.

`context`  

The managed object context into which values will be returned.

## Return Value

An incremental store node encapsulating the persistent external values of the object with object ID `objectID`, or `nil` if the corresponding object cannot be found.

## Discussion

The returned node should include all attributes values and may include to-one relationship values as instances of NSManagedObjectID.

If an object with object ID `objectID` cannot be found, the method should return `nil` and—if `error` is not `NULL`—create and return an appropriate error object in `error`.

## See Also

### Manipulating Managed Objects

func execute(NSPersistentStoreRequest, with: NSManagedObjectContext?) throws -> Any

Returns a value as appropriate for the given request, or nil if the request cannot be completed.

func newValue(forRelationship: NSRelationshipDescription, forObjectWith: NSManagedObjectID, with: NSManagedObjectContext?) throws -> Any

Returns the relationship for the given relationship of the object with a given object ID.

func obtainPermanentIDs(for: [NSManagedObject]) throws -> [NSManagedObjectID]

Returns an array containing the object IDs for a given array of newly-inserted objects.

func newObjectID(for: NSEntityDescription, referenceObject: Any) -> NSManagedObjectID

Returns a new object ID that uses given data as the key.

func referenceObject(for: NSManagedObjectID) -> Any

Returns the reference data used to construct a given object ID.

