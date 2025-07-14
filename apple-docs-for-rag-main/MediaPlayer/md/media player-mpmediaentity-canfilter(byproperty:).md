

- Media Player
- MPMediaEntity
-  canFilter(byProperty:) 

Type Method

# canFilter(byProperty:)

Indicates whether you can use the media property key that you specify to construct a media property predicate.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+tvOS 14.0+visionOS 1.0+

``` source
class func canFilter(byProperty property: String) -> Bool
```

## Parameters 

`property`  

The key for the media property that you want to examine.

## Return Value

true if the property you are testing can be used to construct a media property predicate of type MPMediaPropertyPredicate; otherwise, false.

## Discussion

To see which media property keys you can use with this method, refer to Media entity property keys, General media item property keys, Playlist property keys, and User-defined property keys.

## See Also

### Working with media properties

func enumerateValues(forProperties: Set&lt;String>, using: (String, Any, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Executes a provided block with the fetched values for the given item properties.

var persistentID: MPMediaEntityPersistentID

The persistent identifier for a media entity.

subscript(Any) -> Any?

Returns the object specified by the key.

func value(forProperty: String) -> Any?

Retrieves the value for a specified media property key.

typealias MPMediaEntityPersistentID

Defines the type for storing a persistent identifier to a particular entity.

