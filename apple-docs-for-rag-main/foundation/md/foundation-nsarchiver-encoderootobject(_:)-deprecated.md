

- Foundation
- NSArchiver
-  encodeRootObject(\_:) Deprecated

Instance Method

# encodeRootObject(\_:)

Archives a given object along with all the objects to which it is connected.

iOS 2.0–11.0DeprecatediPadOS 2.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.0–10.13Deprecated

``` source
func encodeRootObject(_ rootObject: Any)
```

Deprecated

Use NSKeyedArchiver instead

## Parameters 

`rootObject`  

The root object of the object graph to archive.

## Discussion

If any object is encountered more than once while traversing the graph, it is encoded only once, but the multiple references to it are stored. (See Archives and Serializations Programming Guide for more information.)

This message must not be sent more than once to a given `NSArchiver` object; an `NSInvalidArgumentException` is raised if a root object has already been encoded. If you need to encode multiple object graphs, therefore, don’t attempt to reuse an `NSArchiver` instance; instead, create a new one for each graph.

## See Also

### Archiving data

class func archivedData(withRootObject: Any) -> Data

Returns a data object containing the encoded form of the object graph whose root object is given.

Deprecated

class func archiveRootObject(Any, toFile: String) -> Bool

Creates a temporary instance of `NSArchiver` and archives an object graph by encoding it into a data object and writing the resulting data object to a specified file.

Deprecated

func encodeConditionalObject(Any?)

Conditionally archives a given object.

Deprecated

