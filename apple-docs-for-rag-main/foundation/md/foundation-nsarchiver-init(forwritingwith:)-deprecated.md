

- Foundation
- NSArchiver
-  init(forWritingWith:) Deprecated

Initializer

# init(forWritingWith:)

Returns an archiver, initialized to encode stream and version information into a given mutable data object.

iOS 2.0–11.0DeprecatediPadOS 2.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.0–10.13Deprecated

``` source
init(forWritingWith mdata: NSMutableData)
```

Deprecated

Use NSKeyedArchiver instead

## Parameters 

`mdata`  

The mutable data object into which to write the archive. This value must not be `nil`.

## Return Value

An archiver object, initialized to encode stream and version information into `data`.

## Discussion

Raises an `NSInvalidArgumentException` if `data` is `nil`.

## See Also

### Related Documentation

var archiverData: NSMutableData

The receiver’s archive data.

Deprecated

Archives and Serializations Programming Guide

