

- WebKit
- WKWebExtension
- WKWebExtension.DataRecord
-  sizeInBytes(ofTypes:) 

Instance Method

# sizeInBytes(ofTypes:)

Retrieves the size in bytes of the specific data types in this data record.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
func sizeInBytes(ofTypes dataTypes: Set) -> Int
```

## Parameters 

`dataTypes`  

The set of data types to measure the size for.

## See Also

### Related Documentation

var totalSizeInBytes: Int

The total size in bytes of all data types contained in this data record.

