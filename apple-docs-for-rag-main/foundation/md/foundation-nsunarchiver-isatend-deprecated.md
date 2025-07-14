

- Foundation
- NSUnarchiver
-  isAtEnd Deprecated

Instance Property

# isAtEnd

A Boolean value that indicates whether the receiver has reached the end of the encoded data while decoding.

iOS 2.0–11.0DeprecatediPadOS 2.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.0–10.13Deprecated

``` source
var isAtEnd: Bool { get }
```

Deprecated

Use NSKeyedUnarchiver instead

## Discussion

true if the receiver has reached the end of the encoded data while decoding, otherwise false.

You can invoke this method after invoking `decodeObject` to discover whether the archive contains extra data following the encoded object graph. If it does, you can either ignore this anomaly or consider it an error.

## See Also

### Managing an NSUnarchiver

var systemVersion: UInt32

The system version number in effect when the archive was created.

Deprecated

