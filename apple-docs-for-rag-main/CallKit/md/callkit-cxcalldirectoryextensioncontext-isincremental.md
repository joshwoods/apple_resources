

- CallKit
- CXCallDirectoryExtensionContext
-  isIncremental 

Instance Property

# isIncremental

A Boolean value that indicates whether the request provides data incrementally.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+visionOS 1.0+

``` source
var isIncremental: Bool { get }
```

## Discussion

Before adding or removing any entries, if you call this method and the value is true, the request must only add or remove entries relative to the last time the system loaded data for the extension. Otherwise, if you don’t call this method, or if the value is false, the request must add the full list of entries without removing any, regardless of whether the system loaded data in the past.

## See Also

### Completing Requests

func completeRequest(completionHandler: ((Bool) -> Void)?)

Completes the request to the extension context.

