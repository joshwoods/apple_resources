

- Media Player
-  MPMediaEntityPersistentID 

Type Alias

# MPMediaEntityPersistentID

Defines the type for storing a persistent identifier to a particular entity.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias MPMediaEntityPersistentID = UInt64
```

## Discussion

The value persists across application launches and across syncs that don’t change the sync status of the media item. The value isn’t guaranteed to persist across a sync/unsync/sync cycle.

## See Also

### Working with media properties

class func canFilter(byProperty: String) -> Bool

Indicates whether you can use the media property key that you specify to construct a media property predicate.

func enumerateValues(forProperties: Set&lt;String>, using: (String, Any, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Executes a provided block with the fetched values for the given item properties.

var persistentID: MPMediaEntityPersistentID

The persistent identifier for a media entity.

subscript(Any) -> Any?

Returns the object specified by the key.

func value(forProperty: String) -> Any?

Retrieves the value for a specified media property key.

