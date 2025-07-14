

- Foundation
- NSUnarchiver
-  init(forReadingWith:) Deprecated

Initializer

# init(forReadingWith:)

Returns an `NSUnarchiver` object initialized to read an archive from a given data object.

iOS 2.0–11.0DeprecatediPadOS 2.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.0–10.13Deprecated

``` source
init?(forReadingWith data: Data)
```

Deprecated

Use NSKeyedUnarchiver instead

## Parameters 

`data`  

The archive data.

## Return Value

An `NSUnarchiver` object initialized to read an archive from `data`. Returns `nil` if `data` is not a valid archive.

## Discussion

The method decodes the system version number that was archived in `data` prepares the `NSUnarchiver` object for a subsequent invocation of decodeObject().

Raises an `NSInvalidArgumentException` if `data` is `nil`.

## See Also

### Related Documentation

Archives and Serializations Programming Guide

var systemVersion: UInt32

The system version number in effect when the archive was created.

Deprecated

