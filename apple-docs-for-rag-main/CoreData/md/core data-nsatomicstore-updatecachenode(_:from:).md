

- Core Data
- NSAtomicStore
-  updateCacheNode(\_:from:) 

Instance Method

# updateCacheNode(\_:from:)

Updates the given cache node using the values in a given managed object.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func updateCacheNode(
    _ node: NSAtomicStoreCacheNode,
    from managedObject: NSManagedObject
)
```

## Parameters 

`node`  

The cache node to update.

`managedObject`  

The managed object with which to update `node`.

## Discussion

This method is invoked by the framework after a save operation on a managed object context, once for each updated `NSManagedObject` instance.

You override this method in a subclass to take the information from `managedObject` and update `node`.

### Special Considerations

You must override this method.

## See Also

### Updating Cache Nodes

func newCacheNode(for: NSManagedObject) -> NSAtomicStoreCacheNode

Returns a new cache node for a given managed object.

func newReferenceObject(for: NSManagedObject) -> Any

Returns a new reference object for a given managed object.

func willRemoveCacheNodes(Set&lt;NSAtomicStoreCacheNode>)

Method invoked before the store removes the given collection of cache nodes.

