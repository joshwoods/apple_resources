

- Core Data
- NSAtomicStore
-  newCacheNode(for:) 

Instance Method

# newCacheNode(for:)

Returns a new cache node for a given managed object.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func newCacheNode(for managedObject: NSManagedObject) -> NSAtomicStoreCacheNode
```

## Parameters 

`managedObject`  

A managed object.

## Return Value

A new cache node for `managedObject`.

## Discussion

This method is invoked by the framework during a save operation, once for each newly-inserted managed object. It should pull information from the managed object and return a cache node containing the information (the node will be registered by the framework).

### Special Considerations

You must override this method.

## See Also

### Updating Cache Nodes

func newReferenceObject(for: NSManagedObject) -> Any

Returns a new reference object for a given managed object.

func updateCacheNode(NSAtomicStoreCacheNode, from: NSManagedObject)

Updates the given cache node using the values in a given managed object.

func willRemoveCacheNodes(Set&lt;NSAtomicStoreCacheNode>)

Method invoked before the store removes the given collection of cache nodes.

