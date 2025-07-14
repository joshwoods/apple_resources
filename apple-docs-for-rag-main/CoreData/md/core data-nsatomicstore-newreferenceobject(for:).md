

- Core Data
- NSAtomicStore
-  newReferenceObject(for:) 

Instance Method

# newReferenceObject(for:)

Returns a new reference object for a given managed object.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func newReferenceObject(for managedObject: NSManagedObject) -> Any
```

## Parameters 

`managedObject`  

A managed object. At the time this method is called, it has a temporary ID.

## Return Value

A new reference object for `managedObject`.

## Discussion

This method is invoked by the framework after a save operation on a managed object context, once for each newly-inserted managed object. The value returned is used to create a permanent ID for the object and must be unique for an instance within its entity’s inheritance hierarchy (in this store).

### Special Considerations

You must override this method.

This method must return a stable (unchanging) value for a given object, otherwise Save As and migration will not work correctly. This means that you can use arbitrary numbers, UUIDs, or other random values only if they are persisted with the raw data. If you cannot save the originally-assigned reference object with the data, then the method must derive the reference object from the managed object’s values. For more details, see Atomic Store Programming Topics.

## See Also

### Updating Cache Nodes

func newCacheNode(for: NSManagedObject) -> NSAtomicStoreCacheNode

Returns a new cache node for a given managed object.

func updateCacheNode(NSAtomicStoreCacheNode, from: NSManagedObject)

Updates the given cache node using the values in a given managed object.

func willRemoveCacheNodes(Set&lt;NSAtomicStoreCacheNode>)

Method invoked before the store removes the given collection of cache nodes.

