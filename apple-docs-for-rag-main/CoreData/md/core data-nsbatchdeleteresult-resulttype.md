

- Core Data
- NSBatchDeleteResult
-  resultType 

Instance Property

# resultType

The data type of the request’s result value.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var resultType: NSBatchDeleteRequestResultType { get }
```

## Discussion

This property’s value is set to the request’s resultType property.

## See Also

### Accessing the Result

var result: Any?

The value the request returns after it executes.

enum NSBatchDeleteRequestResultType

The types of result a batch delete request can provide when it executes.

