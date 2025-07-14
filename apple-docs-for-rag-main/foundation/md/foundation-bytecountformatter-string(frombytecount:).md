

- Foundation
- ByteCountFormatter
-  string(fromByteCount:) 

Instance Method

# string(fromByteCount:)

Converts a byte count into a string without creating an `NSNumber` object.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func string(fromByteCount byteCount: Int64) -> String
```

## Parameters 

`byteCount`  

The byte count.

## Return Value

A string containing the formatted `byteCount` value.

## See Also

### Creating Strings from Byte Count

class func string(fromByteCount: Int64, countStyle: ByteCountFormatter.CountStyle) -> String

Converts a byte count into the specified string format without creating an `NSNumber` object.

