

- Foundation
- NSUnarchiver
-  unarchiveObject(with:) Deprecated

Type Method

# unarchiveObject(with:)

Decodes and returns the object archived in a given `NSData` object.

iOS 2.0–11.0DeprecatediPadOS 2.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.0–10.13Deprecated

``` source
class func unarchiveObject(with data: Data) -> Any?
```

Deprecated

Use NSKeyedUnarchiver instead

## Parameters 

`data`  

An `NSData` object that contains an archive created using `NSArchiver`.

## Return Value

The object, or object graph, that was archived in `data`. Returns `nil` if `data` cannot be unarchived.

## Discussion

This method invokes init(forReadingWith:) and decodeObject() to create a temporary `NSUnarchiver` object that decodes the object. If the archived object is the root of a graph of objects, the entire graph is unarchived.

## See Also

### Related Documentation

func encodeRootObject(Any)

Archives a given object along with all the objects to which it is connected.

Deprecated

### Decoding objects

class func unarchiveObject(withFile: String) -> Any?

Decodes and returns the object archived in the file `path`.

Deprecated

