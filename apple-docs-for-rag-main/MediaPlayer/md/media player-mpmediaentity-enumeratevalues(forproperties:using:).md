

- Media Player
- MPMediaEntity
-  enumerateValues(forProperties:using:) 

Instance Method

# enumerateValues(forProperties:using:)

Executes a provided block with the fetched values for the given item properties.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
func enumerateValues(
    forProperties properties: Set,
    using block: @escaping (String, Any, UnsafeMutablePointer) -> Void
)
```

## Parameters 

`properties`  

A set of property keys that you want the values for.

`block`  

A block object that executes for each fetched property value.

## Discussion

Use this method to get property values in a batch fashion. Anytime the app accesses more than one property, enumerating over a set of property keys is more efficient than fetching each individual property with value(forProperty:).

To see which media property keys you can use with this method, refer to Media entity property keys, General media item property keys, Playlist property keys, and User-defined property keys.

## See Also

### Working with media properties

class func canFilter(byProperty: String) -> Bool

Indicates whether you can use the media property key that you specify to construct a media property predicate.

var persistentID: MPMediaEntityPersistentID

The persistent identifier for a media entity.

subscript(Any) -> Any?

Returns the object specified by the key.

func value(forProperty: String) -> Any?

Retrieves the value for a specified media property key.

typealias MPMediaEntityPersistentID

Defines the type for storing a persistent identifier to a particular entity.

