

- Core Data
- NSAtomicStore
-  objectID(for:withReferenceObject:) 

Instance Method

# objectID(for:withReferenceObject:)

Returns a managed object ID from the reference data for a specified entity.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func objectID(
    for entity: NSEntityDescription,
    withReferenceObject data: Any
) -> NSManagedObjectID
```

## Parameters 

`entity`  

An entity description object.

`data`  

Reference data for which the managed object ID is required.

## Return Value

The managed object ID from the reference data for a specified entity

## Discussion

You use this method to create managed object IDs which are then used to create cache nodes for information being loaded into the store.

### Special Considerations

You should not override this method.

## See Also

### Loading a Store

func load() throws

Loads the cache nodes for the receiver.

func addCacheNodes(Set&lt;NSAtomicStoreCacheNode>)

Registers a set of cache nodes with the receiver.

