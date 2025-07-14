

- Media Player
- MPMediaEntity
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Returns the object specified by the key.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+tvOS 14.0+visionOS 1.0+

``` source
subscript(key: Any) -> Any? { get }
```

## Parameters 

`key`  

The key associated with the retrieved object.

## Return Value

The object that is specified by the key.

## Discussion

The method provides read-only support for Objective-C subscripting syntax with MPMediaEntity property constants.

## See Also

### Working with media properties

class func canFilter(byProperty: String) -> Bool

Indicates whether you can use the media property key that you specify to construct a media property predicate.

func enumerateValues(forProperties: Set&lt;String>, using: (String, Any, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Executes a provided block with the fetched values for the given item properties.

var persistentID: MPMediaEntityPersistentID

The persistent identifier for a media entity.

func value(forProperty: String) -> Any?

Retrieves the value for a specified media property key.

typealias MPMediaEntityPersistentID

Defines the type for storing a persistent identifier to a particular entity.

