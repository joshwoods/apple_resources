

- Core Data
- NSAtomicStoreCacheNode
-  value(forKey:) 

Instance Method

# value(forKey:)

Returns the value for a given key.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func value(forKey key: String) -> Any?
```

## Parameters 

`key`  

The name of a property.

## Return Value

The value for the property named `key`. For an attribute, the return value is an instance of an attribute type supported by Core Data (see NSAttributeDescription); for a to-one relationship, the return value must be another cache node instance; for a to-many relationship, the return value must be an collection of the related cache nodes.

## Discussion

The default implementation forwards the request to the propertyCache dictionary if `key` matches a property name of the entity for the cache node. If `key` does not represent a property, the standard value(forKey:) implementation is used.

## See Also

### Managing Node Data

var objectID: NSManagedObjectID

The managed object ID of the node.

var propertyCache: NSMutableDictionary?

The property cache dictionary of the node.

func setValue(Any?, forKey: String)

Sets the value for the given key.

