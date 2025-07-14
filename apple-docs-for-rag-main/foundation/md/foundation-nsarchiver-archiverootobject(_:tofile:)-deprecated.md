

- Foundation
- NSArchiver
-  archiveRootObject(\_:toFile:) Deprecated

Type Method

# archiveRootObject(\_:toFile:)

Creates a temporary instance of `NSArchiver` and archives an object graph by encoding it into a data object and writing the resulting data object to a specified file.

iOS 2.0–11.0DeprecatediPadOS 2.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.0–10.13Deprecated

``` source
class func archiveRootObject(
    _ rootObject: Any,
    toFile path: String
) -> Bool
```

Deprecated

Use NSKeyedArchiver instead

## Parameters 

`rootObject`  

The root object of the object graph to archive.

`path`  

The location of the file into which to write the archive.

## Return Value

true if the archive was written successfully, otherwise false.

## Discussion

This convenience method invokes archivedData(withRootObject:) to get the encoded data, and then sends that data object the message write(toFile:atomically:), using `path` for the first argument and true for the second.

The archived data should be retrieved from the archive by an NSUnarchiver object.

## See Also

### Related Documentation

func write(toFile: String, atomically: Bool) -> Bool

Writes the data object’s bytes to the file specified by a given path.

### Archiving data

class func archivedData(withRootObject: Any) -> Data

Returns a data object containing the encoded form of the object graph whose root object is given.

Deprecated

func encodeRootObject(Any)

Archives a given object along with all the objects to which it is connected.

Deprecated

func encodeConditionalObject(Any?)

Conditionally archives a given object.

Deprecated

