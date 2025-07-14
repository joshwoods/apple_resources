

- Foundation
- NSUUID
-  uuidString 

Instance Property

# uuidString

The UUID as a string.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var uuidString: String { get }
```

## Discussion

A string containing a formatted UUID for example `E621E1F8-C36C-495A-93FC-0C247A3E6E5F`.

Use this property when you need a string representation of the `NSUUID` object—for example, to compare with a CFUUID object.

## See Also

### Get UUID Values

func getBytes(UnsafeMutablePointer&lt;UInt8>)

Returns the UUID as bytes.

