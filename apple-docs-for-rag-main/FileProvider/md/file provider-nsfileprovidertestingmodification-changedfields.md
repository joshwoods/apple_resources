

- File Provider
- NSFileProviderTestingModification
-  changedFields 

Instance Property

# changedFields

A list of the fields that changed.

iOS 16.0+iPadOS 16.0+macOS 11.3+visionOS 1.0+

``` source
var changedFields: NSFileProviderItemFields { get }
```

**Required**

## See Also

### Accessing the Operation’s Data

var sourceItem: NSFileProviderItem

A description of the source item.

**Required**

var targetSide: NSFileProviderTestingOperationSide

The target location for the modification operation.

**Required**

var targetItemIdentifier: NSFileProviderItemIdentifier

The unique identifier for the target item.

**Required**

var targetItemBaseVersion: NSFileProviderItemVersion

The version of the changed item.

**Required**

var domainVersion: NSFileProviderDomainVersion?

The domain’s version when the change occurred.

**Required**

