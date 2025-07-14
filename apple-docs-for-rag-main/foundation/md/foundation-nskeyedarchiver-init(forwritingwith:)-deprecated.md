

- Foundation
- NSKeyedArchiver
-  init(forWritingWith:) Deprecated

Initializer

# init(forWritingWith:)

Initializes an archiver to encode data into a given a mutable-data object.

iOS 2.0–12.0DeprecatediPadOS 2.0–12.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.2–10.14DeprecatedtvOS 9.0–12.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–5.0Deprecated

``` source
init(forWritingWith data: NSMutableData)
```

Deprecated

Use init(requiringSecureCoding:) instead.

## Parameters 

`data`  

The mutable-data object into which the archive is written.

## Discussion

When you finish encoding data, you must invoke finishEncoding() at which point `data` is filled. The format of the receiver is `NSPropertyListBinaryFormat_v1_0`.

## See Also

### Related Documentation

Archives and Serializations Programming Guide

### Creating a Keyed Archiver

init(requiringSecureCoding: Bool)

Creates an archiver to encode data, and optionally disables secure coding.

init()

Initializes an archiver to encode data.

Deprecated

