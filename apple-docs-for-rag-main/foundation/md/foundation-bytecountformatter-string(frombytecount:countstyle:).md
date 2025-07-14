

- Foundation
- ByteCountFormatter
-  string(fromByteCount:countStyle:) 

Type Method

# string(fromByteCount:countStyle:)

Converts a byte count into the specified string format without creating an `NSNumber` object.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func string(
    fromByteCount byteCount: Int64,
    countStyle: ByteCountFormatter.CountStyle
) -> String
```

## Parameters 

`byteCount`  

The byte count.

`countStyle`  

The formatter style. See ByteCountFormatter.CountStyle for possible values.

## Return Value

A string containing the formatted `byteCount` value.

## See Also

### Related Documentation

Data Formatting Guide

### Creating Strings from Byte Count

func string(fromByteCount: Int64) -> String

Converts a byte count into a string without creating an `NSNumber` object.

