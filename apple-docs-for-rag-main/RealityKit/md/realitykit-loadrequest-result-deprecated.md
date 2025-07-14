

- RealityKit
- LoadRequest
-  result Deprecated

Instance Property

# result

The result of the load operation.

iOS 13.0–18.0DeprecatediPadOS 13.0–18.0DeprecatedMac Catalyst 13.0–18.0DeprecatedmacOS 10.15–15.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
var result: Result? { get }
```

## Discussion

A load operation can have the following results:

- `success(Output)` … The load operation has completed successfully.

- `failure(Error)` … The load operation failed.

- `nil` … The load operation is still in progress.

