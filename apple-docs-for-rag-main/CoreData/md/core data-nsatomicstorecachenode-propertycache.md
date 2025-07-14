

- Core Data
- NSAtomicStoreCacheNode
-  propertyCache 

Instance Property

# propertyCache

The property cache dictionary of the node.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var propertyCache: NSMutableDictionary? { get set }
```

## Discussion

This dictionary is used by value(forKey:) and setValue(_:forKey:) for property values. This property is `nil` unless it has been explicitly set or non-`nil` values have been set for keys using setValue(_:forKey:).

## See Also

### Managing Node Data

var objectID: NSManagedObjectID

The managed object ID of the node.

func value(forKey: String) -> Any?

Returns the value for a given key.

func setValue(Any?, forKey: String)

Sets the value for the given key.

