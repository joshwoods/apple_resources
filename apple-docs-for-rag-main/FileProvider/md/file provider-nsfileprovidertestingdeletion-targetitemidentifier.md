

- File Provider
- NSFileProviderTestingDeletion
-  targetItemIdentifier 

Instance Property

# targetItemIdentifier

The unique identifier for the target item.

iOS 16.0+iPadOS 16.0+macOS 11.3+visionOS 1.0+

``` source
var targetItemIdentifier: NSFileProviderItemIdentifier { get }
```

**Required**

## See Also

### Accessing the Operation’s Data

var sourceItemIdentifier: NSFileProviderItemIdentifier

The unique identifier for the source item.

**Required**

var targetSide: NSFileProviderTestingOperationSide

The target location for the delete operation.

**Required**

var targetItemBaseVersion: NSFileProviderItemVersion

The version of the deleted item.

**Required**

var domainVersion: NSFileProviderDomainVersion?

The domain’s version when the source location deleted the item.

**Required**

