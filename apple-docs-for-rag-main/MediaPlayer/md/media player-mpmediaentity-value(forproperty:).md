

- Media Player
- MPMediaEntity
-  value(forProperty:) 

Instance Method

# value(forProperty:)

Retrieves the value for a specified media property key.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+tvOS 14.0+visionOS 1.0+

``` source
func value(forProperty property: String) -> Any?
```

## Parameters 

`property`  

The media property key that you want the corresponding value of.

## Return Value

The value for the media `property` key.

## Discussion

Use enumerateValues(forProperties:using:) to efficiently access more than one property at a time.

To see which media property keys you can use with this method, refer to Media entity property keys, General media item property keys, Playlist property keys, and User-defined property keys.

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

typealias MPMediaEntityPersistentID

Defines the type for storing a persistent identifier to a particular entity.

