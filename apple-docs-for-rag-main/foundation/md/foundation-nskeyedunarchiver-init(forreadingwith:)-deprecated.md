

- Foundation
- NSKeyedUnarchiver
-  init(forReadingWith:) Deprecated

Initializer

# init(forReadingWith:)

Initializes an archiver to decode data from the specified location.

iOS 2.0–12.0DeprecatediPadOS 2.0–12.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.2–10.14DeprecatedtvOS 9.0–12.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–5.0Deprecated

``` source
init(forReadingWith data: Data)
```

Deprecated

Use init(forReadingFrom:) instead.

## Parameters 

`data`  

An archive previously encoded by NSKeyedArchiver.

## Return Value

An NSKeyedUnarchiver object initialized for for decoding `data`.

## Discussion

When you finish decoding data, you should invoke finishDecoding().

This method throws an exception if `data` is not a valid archive.

## See Also

### Related Documentation

Archives and Serializations Programming Guide

### Creating a Keyed Unarchiver

init(forReadingFrom: Data) throws

Initializes an archiver to decode data from the specified location.

init()

Initializes an archiver to decode data.

Deprecated

