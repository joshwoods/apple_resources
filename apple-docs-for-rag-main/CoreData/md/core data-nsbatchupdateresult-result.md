

- Core Data
- NSBatchUpdateResult
-  result 

Instance Property

# result

The result of a batch-update request, either the number of updated objects, the identifiers of the updated objects, or a status value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var result: Any? { get }
```

## See Also

### Accessing Results

var resultType: NSBatchUpdateRequestResultType

The type of result that Core Data returns from the request.

enum NSBatchUpdateRequestResultType

Result types for a batch-update request.

