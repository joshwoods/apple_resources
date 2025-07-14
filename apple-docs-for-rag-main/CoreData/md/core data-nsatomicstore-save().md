

- Core Data
- NSAtomicStore
-  save() 

Instance Method

# save()

Saves the cache nodes.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func save() throws
```

## Discussion

You override this method to make persistent the necessary information from the cache nodes to the URL specified for the receiver.

### Special Considerations

You must override this method.

## See Also

### Related Documentation

func updateCacheNode(NSAtomicStoreCacheNode, from: NSManagedObject)

Updates the given cache node using the values in a given managed object.

func willRemoveCacheNodes(Set&lt;NSAtomicStoreCacheNode>)

Method invoked before the store removes the given collection of cache nodes.

func newReferenceObject(for: NSManagedObject) -> Any

Returns a new reference object for a given managed object.

