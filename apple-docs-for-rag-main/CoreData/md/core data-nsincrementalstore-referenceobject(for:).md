

- Core Data
- NSIncrementalStore
-  referenceObject(for:) 

Instance Method

# referenceObject(for:)

Returns the reference data used to construct a given object ID.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func referenceObject(for objectID: NSManagedObjectID) -> Any
```

## Parameters 

`objectID`  

An object ID created by the receiver.

## Return Value

The reference data used to construct objectID.

## Discussion

This method raises an invalidArgumentException if the object ID was not created by the receiving store.

You should not override this method.

## See Also

### Manipulating Managed Objects

func execute(NSPersistentStoreRequest, with: NSManagedObjectContext?) throws -> Any

Returns a value as appropriate for the given request, or nil if the request cannot be completed.

func newValuesForObject(with: NSManagedObjectID, with: NSManagedObjectContext) throws -> NSIncrementalStoreNode

Returns an incremental store node encapsulating the persistent external values of the object with a given object ID.

func newValue(forRelationship: NSRelationshipDescription, forObjectWith: NSManagedObjectID, with: NSManagedObjectContext?) throws -> Any

Returns the relationship for the given relationship of the object with a given object ID.

func obtainPermanentIDs(for: [NSManagedObject]) throws -> [NSManagedObjectID]

Returns an array containing the object IDs for a given array of newly-inserted objects.

func newObjectID(for: NSEntityDescription, referenceObject: Any) -> NSManagedObjectID

Returns a new object ID that uses given data as the key.

