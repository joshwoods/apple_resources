

- Core Data
- NSAtomicStoreCacheNode
-  setValue(\_:forKey:) 

Instance Method

# setValue(\_:forKey:)

Sets the value for the given key.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func setValue(
    _ value: Any?,
    forKey key: String
)
```

## Parameters 

`value`  

The value for the property identified by `key`.

`key`  

The name of a property.

## Discussion

The default implementation forwards the request to the propertyCache dictionary if `key` matches a property name of the entity for this cache node. If `key` does not represent a property, the standard setValue(_:forKey:) implementation is used.

## See Also

### Managing Node Data

var objectID: NSManagedObjectID

The managed object ID of the node.

var propertyCache: NSMutableDictionary?

The property cache dictionary of the node.

func value(forKey: String) -> Any?

Returns the value for a given key.

