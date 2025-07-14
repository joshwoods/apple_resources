

- Core Data
- NSIncrementalStore
-  newObjectID(for:referenceObject:) 

Instance Method

# newObjectID(for:referenceObject:)

Returns a new object ID that uses given data as the key.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func newObjectID(
    for entity: NSEntityDescription,
    referenceObject data: Any
) -> NSManagedObjectID
```

## Parameters 

`entity`  

The entity for the new object ID.

`data`  

An object of type NSString or NSNumber to use as the key.

## Return Value

A new object ID for an instance of the entity specified by `entity` and that uses `data` as the key.

## Discussion

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

func referenceObject(for: NSManagedObjectID) -> Any

Returns the reference data used to construct a given object ID.

