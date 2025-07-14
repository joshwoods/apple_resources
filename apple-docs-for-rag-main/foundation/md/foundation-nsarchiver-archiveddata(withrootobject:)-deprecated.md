

- Foundation
- NSArchiver
-  archivedData(withRootObject:) Deprecated

Type Method

# archivedData(withRootObject:)

Returns a data object containing the encoded form of the object graph whose root object is given.

iOS 2.0–11.0DeprecatediPadOS 2.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.0–10.13Deprecated

``` source
class func archivedData(withRootObject rootObject: Any) -> Data
```

Deprecated

Use NSKeyedArchiver instead

## Parameters 

`rootObject`  

The root object of the object graph to archive.

## Return Value

A data object containing the encoded form of the object graph whose root object is `rootObject`.

## Discussion

This method invokes init(forWritingWith:) and encodeRootObject(_:) to create a temporary archiver that encodes the object graph.

## See Also

### Related Documentation

init(forWritingWith: NSMutableData)

Returns an archiver, initialized to encode stream and version information into a given mutable data object.

Deprecated

### Archiving data

class func archiveRootObject(Any, toFile: String) -> Bool

Creates a temporary instance of `NSArchiver` and archives an object graph by encoding it into a data object and writing the resulting data object to a specified file.

Deprecated

func encodeRootObject(Any)

Archives a given object along with all the objects to which it is connected.

Deprecated

func encodeConditionalObject(Any?)

Conditionally archives a given object.

Deprecated

