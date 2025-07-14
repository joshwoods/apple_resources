

- Core Data
- NSIncrementalStore
-  obtainPermanentIDs(for:) 

Instance Method

# obtainPermanentIDs(for:)

Returns an array containing the object IDs for a given array of newly-inserted objects.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func obtainPermanentIDs(for array: [NSManagedObject]) throws -> [NSManagedObjectID]
```

## Parameters 

`array`  

An array of newly-inserted objects.

## Return Value

An array containing the object IDs for the objects in `array`.

## Discussion

The returned array must return the object IDs in the same order as the objects appear in `array`.

## Discussion

This method is called before execute(_:with:) with a save request, to assign permanent IDs to newly-inserted objects.

## See Also

### Manipulating Managed Objects

func execute(NSPersistentStoreRequest, with: NSManagedObjectContext?) throws -> Any

Returns a value as appropriate for the given request, or nil if the request cannot be completed.

func newValuesForObject(with: NSManagedObjectID, with: NSManagedObjectContext) throws -> NSIncrementalStoreNode

Returns an incremental store node encapsulating the persistent external values of the object with a given object ID.

func newValue(forRelationship: NSRelationshipDescription, forObjectWith: NSManagedObjectID, with: NSManagedObjectContext?) throws -> Any

Returns the relationship for the given relationship of the object with a given object ID.

func newObjectID(for: NSEntityDescription, referenceObject: Any) -> NSManagedObjectID

Returns a new object ID that uses given data as the key.

func referenceObject(for: NSManagedObjectID) -> Any

Returns the reference data used to construct a given object ID.

