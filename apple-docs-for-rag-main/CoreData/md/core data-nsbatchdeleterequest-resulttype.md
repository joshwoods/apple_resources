

- Core Data
- NSBatchDeleteRequest
-  resultType 

Instance Property

# resultType

The type of result the request provides when it executes.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var resultType: NSBatchDeleteRequestResultType { get set }
```

## Discussion

Set this property before you execute the request if you require a result type other than the default of NSBatchDeleteRequestResultType.resultTypeStatusOnly.

## See Also

### Configuring the Result Type

enum NSBatchDeleteRequestResultType

The types of result a batch delete request can provide when it executes.

