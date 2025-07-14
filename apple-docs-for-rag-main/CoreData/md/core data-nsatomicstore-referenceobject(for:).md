

- Core Data
- NSAtomicStore
-  referenceObject(for:) 

Instance Method

# referenceObject(for:)

Returns the reference object for a given managed object ID.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func referenceObject(for objectID: NSManagedObjectID) -> Any
```

## Parameters 

`objectID`  

A managed object ID.

## Return Value

The reference object for `objectID`.

## Discussion

Subclasses should invoke this method to extract the reference data from the object ID for each cache node if the data is to be made persistent.

## See Also

### Utility Methods

func cacheNodes() -> Set&lt;NSAtomicStoreCacheNode>

Returns the set of cache nodes registered with the receiver.

func cacheNode(for: NSManagedObjectID) -> NSAtomicStoreCacheNode?

Returns the cache node for a given managed object ID.

