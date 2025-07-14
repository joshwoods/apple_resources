

- Core Data
- NSAtomicStore
-  addCacheNodes(\_:) 

Instance Method

# addCacheNodes(\_:)

Registers a set of cache nodes with the receiver.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func addCacheNodes(_ cacheNodes: Set)
```

## Parameters 

`cacheNodes`  

A set of cache nodes.

## Discussion

You should invoke this method in a subclass during the call to load() to register the loaded information with the store.

## See Also

### Loading a Store

func load() throws

Loads the cache nodes for the receiver.

func objectID(for: NSEntityDescription, withReferenceObject: Any) -> NSManagedObjectID

Returns a managed object ID from the reference data for a specified entity.

