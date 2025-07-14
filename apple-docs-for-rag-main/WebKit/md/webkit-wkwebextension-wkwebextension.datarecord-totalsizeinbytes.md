

- WebKit
- WKWebExtension
- WKWebExtension.DataRecord
-  totalSizeInBytes 

Instance Property

# totalSizeInBytes

The total size in bytes of all data types contained in this data record.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
var totalSizeInBytes: Int { get }
```

## See Also

### Related Documentation

func sizeInBytes(ofTypes: Set&lt;WKWebExtension.DataType>) -> Int

Retrieves the size in bytes of the specific data types in this data record.

