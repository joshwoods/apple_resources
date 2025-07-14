

- Core Data
- NSAtomicStore
-  cacheNodes() 

Instance Method

# cacheNodes()

Returns the set of cache nodes registered with the receiver.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func cacheNodes() -> Set
```

## Return Value

The set of cache nodes registered with the receiver.

## Discussion

You should modify this collection using addCacheNodes(_:): and willRemoveCacheNodes(_:).

## See Also

### Utility Methods

func cacheNode(for: NSManagedObjectID) -> NSAtomicStoreCacheNode?

Returns the cache node for a given managed object ID.

func referenceObject(for: NSManagedObjectID) -> Any

Returns the reference object for a given managed object ID.

