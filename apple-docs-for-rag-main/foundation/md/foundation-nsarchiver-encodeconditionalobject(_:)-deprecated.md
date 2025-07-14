

- Foundation
- NSArchiver
-  encodeConditionalObject(\_:) Deprecated

Instance Method

# encodeConditionalObject(\_:)

Conditionally archives a given object.

iOS 2.0–11.0DeprecatediPadOS 2.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.0–10.13Deprecated

``` source
func encodeConditionalObject(_ object: Any?)
```

Deprecated

Use NSKeyedArchiver instead

## Parameters 

`object`  

The object to archive.

## Discussion

This method overrides the superclass implementation to allow `object` to be encoded only if it is also encoded unconditionally by another object in the object graph. Conditional encoding lets you encode one part of a graph detached from the rest. (See Archives and Serializations Programming Guide for more information.)

This method should be invoked only from within an encode(with:) method. If `object` is `nil`, the `NSArchiver` object encodes it unconditionally as `nil`. This method raises an `NSInvalidArgumentException` if no root object has been encoded.

## See Also

### Archiving data

class func archivedData(withRootObject: Any) -> Data

Returns a data object containing the encoded form of the object graph whose root object is given.

Deprecated

class func archiveRootObject(Any, toFile: String) -> Bool

Creates a temporary instance of `NSArchiver` and archives an object graph by encoding it into a data object and writing the resulting data object to a specified file.

Deprecated

func encodeRootObject(Any)

Archives a given object along with all the objects to which it is connected.

Deprecated

