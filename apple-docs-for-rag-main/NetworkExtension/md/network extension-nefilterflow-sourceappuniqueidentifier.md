

- Network Extension
- NEFilterFlow
-  sourceAppUniqueIdentifier 

Instance Property

# sourceAppUniqueIdentifier

A byte string that uniquely identifies the binary for each build of the app that is the source of the flow.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
var sourceAppUniqueIdentifier: Data? { get }
```

## See Also

### Source app identification

var sourceAppIdentifier: String?

A string containing the identifier of the source app of the flow.

var sourceAppVersion: String?

The short version string of the app that is the source of the flow.

var sourceAppAuditToken: Data?

The audit token of the source application of the flow.

var sourceProcessAuditToken: Data?

The audit token of the process that created the flow.

