

- Core Data
- NSIncrementalStore
-  newValue(forRelationship:forObjectWith:with:) 

Instance Method

# newValue(forRelationship:forObjectWith:with:)

Returns the relationship for the given relationship of the object with a given object ID.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func newValue(
    forRelationship relationship: NSRelationshipDescription,
    forObjectWith objectID: NSManagedObjectID,
    with context: NSManagedObjectContext?
) throws -> Any
```

## Parameters 

`relationship`  

The relationship for which values are requested.

`objectID`  

The ID of the object for which values are requested.

`context`  

The managed object context into which values will be returned.

## Return Value

The value of the relationship specified `relationship` of the object with object ID `objectID`, or `nil` if an error occurs.

## Discussion

If the relationship is a to-one, the method should return an NSManagedObjectID instance that identifies the destination, or an instance of NSNull if the relationship value is `nil`.

If the relationship is a to-many, the method should return a collection object containing NSManagedObjectID instances to identify the related objects. Using an `NSArray` instance is preferred because it will be the most efficient. A store may also return an instance of `NSSet` or `NSOrderedSet`; an instance of `NSDictionary` is not acceptable.

If an object with object ID `objectID` cannot be found, the method should return `nil` and—if `error` is not `NULL`—create and return an appropriate error object in `error`.

## See Also

### Manipulating Managed Objects

func execute(NSPersistentStoreRequest, with: NSManagedObjectContext?) throws -> Any

Returns a value as appropriate for the given request, or nil if the request cannot be completed.

func newValuesForObject(with: NSManagedObjectID, with: NSManagedObjectContext) throws -> NSIncrementalStoreNode

Returns an incremental store node encapsulating the persistent external values of the object with a given object ID.

func obtainPermanentIDs(for: [NSManagedObject]) throws -> [NSManagedObjectID]

Returns an array containing the object IDs for a given array of newly-inserted objects.

func newObjectID(for: NSEntityDescription, referenceObject: Any) -> NSManagedObjectID

Returns a new object ID that uses given data as the key.

func referenceObject(for: NSManagedObjectID) -> Any

Returns the reference data used to construct a given object ID.

