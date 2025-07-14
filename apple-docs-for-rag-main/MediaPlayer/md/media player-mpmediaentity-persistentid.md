

- Media Player
- MPMediaEntity
-  persistentID 

Instance Property

# persistentID

The persistent identifier for a media entity.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOS 14.0+visionOS 1.0+

``` source
var persistentID: MPMediaEntityPersistentID { get }
```

## See Also

### Working with media properties

class func canFilter(byProperty: String) -> Bool

Indicates whether you can use the media property key that you specify to construct a media property predicate.

func enumerateValues(forProperties: Set&lt;String>, using: (String, Any, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Executes a provided block with the fetched values for the given item properties.

subscript(Any) -> Any?

Returns the object specified by the key.

func value(forProperty: String) -> Any?

Retrieves the value for a specified media property key.

typealias MPMediaEntityPersistentID

Defines the type for storing a persistent identifier to a particular entity.

