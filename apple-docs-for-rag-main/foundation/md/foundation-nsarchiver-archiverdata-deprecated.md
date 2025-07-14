

- Foundation
- NSArchiver
-  archiverData Deprecated

Instance Property

# archiverData

The receiver’s archive data.

iOS 2.0–11.0DeprecatediPadOS 2.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.0–10.13Deprecated

``` source
var archiverData: NSMutableData { get }
```

Deprecated

Use NSKeyedArchiver instead

## Discussion

The returned data object is the same one specified as the argument to init(forWritingWith:). It contains whatever data has been encoded thus far by invocations of the various encoding methods. It is safest not to invoke this method until after encodeRootObject(_:) has returned. In other words, although it is possible for a class to invoke this method from within its encode(with:) method, that method must not alter the data.

