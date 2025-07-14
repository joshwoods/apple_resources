

- Network Extension
- NEFilterFlow
-  sourceAppVersion 

Instance Property

# sourceAppVersion

The short version string of the app that is the source of the flow.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
var sourceAppVersion: String? { get }
```

## Discussion

This property is `nil` if the app info is unavailable.

## See Also

### Source app identification

var sourceAppUniqueIdentifier: Data?

A byte string that uniquely identifies the binary for each build of the app that is the source of the flow.

var sourceAppIdentifier: String?

A string containing the identifier of the source app of the flow.

var sourceAppAuditToken: Data?

The audit token of the source application of the flow.

var sourceProcessAuditToken: Data?

The audit token of the process that created the flow.

