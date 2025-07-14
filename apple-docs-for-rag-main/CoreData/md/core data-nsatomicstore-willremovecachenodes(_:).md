

- Core Data
- NSAtomicStore
-  willRemoveCacheNodes(\_:) 

Instance Method

# willRemoveCacheNodes(\_:)

Method invoked before the store removes the given collection of cache nodes.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func willRemoveCacheNodes(_ cacheNodes: Set)
```

## Parameters 

`cacheNodes`  

The set of cache nodes to remove.

## Discussion

This method is invoked by the store before the call to save() with the collection of cache nodes marked as deleted by a managed object context. You can override this method to track the nodes which will not be made persistent in the save() method.

You should not invoke this method directly in a subclass.

## See Also

### Related Documentation

func save() throws

Saves the cache nodes.

### Updating Cache Nodes

func newCacheNode(for: NSManagedObject) -> NSAtomicStoreCacheNode

Returns a new cache node for a given managed object.

func newReferenceObject(for: NSManagedObject) -> Any

Returns a new reference object for a given managed object.

func updateCacheNode(NSAtomicStoreCacheNode, from: NSManagedObject)

Updates the given cache node using the values in a given managed object.

