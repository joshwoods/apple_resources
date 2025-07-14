

- Core Data
- NSAtomicStore
-  cacheNode(for:) 

Instance Method

# cacheNode(for:)

Returns the cache node for a given managed object ID.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func cacheNode(for objectID: NSManagedObjectID) -> NSAtomicStoreCacheNode?
```

## Parameters 

`objectID`  

A managed object ID.

## Return Value

The cache node for `objectID`.

## Discussion

This method is normally used by cache nodes to locate related cache nodes (by relationships).

## See Also

### Utility Methods

func cacheNodes() -> Set&lt;NSAtomicStoreCacheNode>

Returns the set of cache nodes registered with the receiver.

func referenceObject(for: NSManagedObjectID) -> Any

Returns the reference object for a given managed object ID.

